"Clickr"
## Database Schema Design -

[link to schema](https://dbdiagram.io/d/Flickr-db-diagram-65be93daac844320ae60c67c)

## API Documentation

## USER AUTHENTICATION/AUTHORIZATION
Sign Up -
app.route('/', methods="POST')

Login -
app.route('/')
    Invalid Credentials:
    Error message: "Access Denied"
    Status Code: 403

Delete - 
app.route('/', methods="DELETE')

# Photos-
# Users should be able to view all posted photos.
app.route('/')
# Get photos for the current user
app.route('/current')

# Users should be able to create new posts.
app.route('/', methods=["GET","POST"])

# Users should be able to update their posts.
app.route('/photos/photoId', methods=["GET","PUT"])

# Users should be able to delete their posts.
app.route('/photos/photoId', methods=["DELETE'])


# Albums-
# Users should be able to create new albums.
app.route('/', methods=["GET","POST"])

# Users should be able to update their albums.
app.route('/albums/:albumId', methods=["GET","PUT"])

# Users should be able to delete their albums.
app.route('/albums/:albumId'', methods=["DELETE'])


# Comments-
# Users should be able to view all comments on a Photo.
app.route('/comments')

# Users should be able to create new comments on a photo.
app.route('/photos/:photoId/comments', methods=["GET","POST"])

# Users should be able to update their comments on a photo.
app.route('/comments/:commentId', methods=["GET","PUT"])

# Users should be able to delete their comment from a photo.
app.route('/comments/:commentId', methods=["DELETE"])


# Favorites-
# Users should be able to see all photos they favorited.
app.route('/:userId/favorites')

# Users should be able to favorite multiple photos.
# Users should be able to unfavorite photos.

