## uerData Model

Don't get confused with `userData` and `UserData` within the application. `userData` is the Model and `UserData` is usually a declared variable for parsing data to the view or form.

ie: To learn more about already declared variables [look here]()

The `userData` model is a `belongTo`:`user` eloquent model. An additional user model for users information.

### Relational Models

 - `user` parent Model

```php
public function user(){
    return $this->belongsTo('App\User');
}
```

### Accessing userData model

Using a simple Object oriented approach we can chain our userData model.

```php
$user->userData();
```




