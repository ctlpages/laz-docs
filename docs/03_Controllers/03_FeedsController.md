## FeedsController

This controller creates and destroys user posted updates within their news feed.

### Routes

The FeedsController uses these resources:

- store
- destroy

#### store

The `store` resource using verb `POST` creates new user post that in collection populates on assigned user feed on their profile and dashboard.

#### destroy

The `destroy` resource using verb `DELETE` removes the selected user post from the assigned user feed.

