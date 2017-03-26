## User Model

This model controls the `users` table of the application (see `database/migration/CreateUsersTable.php` for migration file). Using Eloquent ORM for database interaction you can add and remove tables to the `protected $fillable` declaration.

The User model is considered the base model seeing that the application revolves around the user, its fair to state that all prebuilt modules and model relationships be owned by the User model.

### Declared Methods

#### setDobAttribute
`setDobAttribute` responsible for converting `_dob` value into unix format. (`setDobAttribute` comes with an `$dob` arguement)

```php
protected function setDobAttribute($dob)
```
#### getAge
`getAge` responsible for calculating users age

```php
protected function getAge()
```
#### scopeUsername
`scopeUsername` returns user value based on `username` search

- Arguement 2 accepts the searched username value.

```php
public function scopeUsername($query, $value)
```

### Relational Models

#### userData
 - `userData` Has One ORM relationship (an extended model for holding additional user information).

```php
public function userData(){
    return $this->hasOne('App\userData');
}
```

#### usersPhotos
 - `usersPhotos` Has Many ORM relationship.

```php
public function usersPhotos(){
    return $this->hasMany('App\UsersPhotos');
}
```

#### online
 - `online` Has One ORM relationship.

```php
public function online(){
    return $this->hasOne('App\Online');
}
```

