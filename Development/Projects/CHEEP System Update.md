- [x] Add Looping Comments
- [x] Edit Comment

- [x] Add Restriction Duration

- [x] Reject Verification
	- admin has the option not to verify the account
	- if admin does not verify the account, it will be deleted.
	- when the rejected user logs in, they will be notified that they have been rejected, then the account will be deleted
	- Steps:
		- [x] add nullable to verified, false if deleted, true if verified
		- [x] delete account button
		- [x] update middleware
			- [x] unverified
			- [x] verified
			- [x] deleted

- [x] Create Admin Announcements
	- announcements is in the chat message
	- when admin makes announcements, it will be directed towards all the users, individually
	- Steps:
		- [x] Create Announcements Page in Admin
		- [x] Store Announcement as message and link to all users
		- [x] Create Announcements Page in Users

- [x] new message indicator 
	- indicates if you have unread messages
	- disappears if you read your messages
	- Steps:
		- [x] Add Read Attribute to messages in
		- [x] When user clicks on message navigation, update all messages as read

- [x] like message
	- [x] liked attribute in messages table

- [x] Forum Categories Set categories
	- subject categories
	- essentially a filtering of categories

- [x] Report Messages
	- [x] Report Form
	- [x] Restricted Boolean in Report migration
	- [x] Restriction Timer

- [x] Restrict Comment
	- [x] Restrict button
	- [x] Restrict Form
	- [x] Restrict Timer
	- [x] Restrict a Comment, where it cannot be viewed