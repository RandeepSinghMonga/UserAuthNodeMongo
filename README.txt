README

Steps to start app locally.

Ensure you have node.js, mongodb.
Start a server.
	# using python
	python -m SimpleHTTPServer 9393
Start node.js server. (Make sure you have started mongo db server before this step)
	# redirect to directory
	node server.js
Open localhost. Go to http://localhost:9393/leafwearablesSignup.html and signup username.
Go to http://localhost:9393/leafwearables.html for sign in and check for existing user and non-existing user.

Approach
The server checks the username/password on signin and if a user exists, returns a json web token to the front-end. The frontend would use this token for any authenticated requests made after this to the server.
