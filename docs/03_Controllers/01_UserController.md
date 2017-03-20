## UserController

This controller oversees everything pertaining to the users profile. The Dashboard/Home Page, Users Profile are maintained in this controller.

### Routes

The UserController uses these resources:

- index
- home
- upload
- dp


#### index

The `index` resource shows a specific user profile within the uri.

For example, within the address bar you would see `http://example.com/_BrianDoe`. `BrianDoe` is the user saved `username` within the users database

#### home

The `home` resource shows the view of the authenticated user dashboard.

#### upload

The `upload` resource using the verb `POST` to upload users photos. For more information view [UsersPhotos Model](02_Models/03_UserPhotos.md)

#### dp

The `dp` resource using the verb `POST` to upload the users default profile picture. For more information view [UsersPhotos Model](02_Models/03_UserPhotos.md)

