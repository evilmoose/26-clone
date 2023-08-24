1. User
   - id (Primary Key)
   - email
   - username
   - image_url
   - header_image_url
   - bio
   - location
   - password
   |-----------------|
   |  messages       | ----> Message
   |-----------------|
   |  followers      | ----> User
   |-----------------|
   |  following      | ----> User

2. Message
   - id (Primary Key)
   - text
   - timestamp
   - user_id (Foreign Key to User)

3. Follows
   - user_being_followed_id (Foreign Key to User)
   - user_following_id (Foreign Key to User)

4. Likes
   - id (Primary Key)
   - user_id (Foreign Key to User)
   - message_id (Foreign Key to Message)
