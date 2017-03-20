## UsersPhotos

`UserPhotos` model contains all users uploaded images.


### Relational Models

`user` parent model

```php
public function user(){
    return $this->belongsTo('App\User');
}
```

### Declared Methods

`UsersUploadedImages` uploades and renames users images.

- Arguement 1 is an `laravel\framework\Illuminate\Http\Uploaded` class
- Arguement 2 is the `App\User` class

```php
public function UserProfilePicture(UploadedFile $file, User $user)
```


`UserProfilePicture` uploads and renames users default profile picture.

- Arguement 1 is an `laravel\framework\Illuminate\Http\Uploaded` class
- Arguement 2 is the `App\User` class

```php
public function UserProfilePicture(UploadedFile $file, User $user)
```

ie: `UserProfilePicture` saves image links in `userData` model. Look at line 71
```php
$user->userData()->update()
```

**(If you want to use a remote or cloud service you should edit `UserProfilePicture` and `UserProfilePicture` methods)**




