## FavController

This controller is responsible for favoriting and unfavoriting authenticated users

### Routes

The FavController uses these resources:

- index
- store
- destroy

#### index

The `index` resource using verb `GET` previews a list of users who favorited you and who you favorited

#### store

The `store` resource using verb `POST` to create a fav from one authenticated user to another.

#### destroy

The `destroy` resource using verb `DELETE` removes the favoriting from one authenticated user to another.

