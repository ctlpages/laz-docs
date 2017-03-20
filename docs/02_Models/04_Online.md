## Online Model

The Online model uses user sessions to capture their last activity. Its a beautiful feature which can be extended for more powerful usage.

### Declared Methods

`scopeOnlineUsers` list users with latest activity.

 - Arguement 2 accepts an integer timelimit.

```php
public function scopeOnlineUsers($query, $timeLimit = 10)
```

`scopeRegistered` returns registered users with latest activity.

 - Arguement 2 accepts an integer timelimit.

```php
public function scopeRegistered($query, $timeLimit = 10)
```

`scopeUpdateIdleUser` updates idle user `last_activity` value

```php
public function scopeUpdateIdleUser($query)
```

### Relational Models

`user` parent Model

```php
public function user(){
    return $this->belongsTo('App\User');
}
```