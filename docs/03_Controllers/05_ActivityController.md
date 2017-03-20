## ActivityController

This controller is responsible previewing all things related to the users account.

### Routes

The ActivityController uses these resources:

- show
- markBellAsRead

#### show

The `show` resource using verb `GET` previews all activity related to the authenticated user

#### markBellAsRead

This `markBellAsRead` using verb `POST` once uri is hit marks all notifications as read.