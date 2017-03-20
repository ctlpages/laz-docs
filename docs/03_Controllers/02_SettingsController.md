## SettingsController

This controller oversees all features in the settings page of the users profile.

### Routes

The Settings Controller only has two actions:

 - edit
 - update

 #### edit

 The `edit` resource previews a specific view page for the authenticated user

 #### update

 The `update` resource using the verb `PUT/PATCH`, updating the information within the users table

 ### Extending the Controller

 For extending the resources of the controller you would just have to add `index`, `create`, `store`, `show` or `destroy`. I will use `destroy` as an example.


Within your `routes.php` file add `destroy` to the list
 ```php
Route::resource('settings', 'SettingsController',
                ['only' => ['edit', 'update', 'destroy']]);
 ```

 Within the `SettingsController` add:

 ```php
public function destroy(){

}
 ```
