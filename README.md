# node-restfulJS

To run the node server, either user git bash or run the command line from the folder this project is in using the command 'node run'

Once you have done this you should get the message
'Mischief occurs on port 8080
Connected to MongoDB'

The server will be up and running and if you make any request you should see a message in the console.

The API lives on http://localhost:8080/api


here are the endpoints, and what verb you will need and what it does for you.

(GET)
/api/bears
-- this will get you all of the bears on the mongodb

(POST)
/api/bears
-- this will post a bear to the mongodb, you will need to look in the body of the post request we use x-www-form-urlencoded
-- the key is name and the value is the name of your bear

(GET)
/api/bears/{bear_id}
-- this will get you the specific bear by id, you get the id either when you post a new bear or you can see all the id by using get on bears


(PUT)
/api/bears/{bear_id}
-- this will update a bear, currently this should only allow you to update the name of the bear

(DELETE)
/api/bears/{bear_id}
-- this will remove the bear from the database, this is a WIP as I'm trying to hold the name of the bear for the message.


TL;DR

Route	                HTTP Verb           	  Description
/api/bears	          GET	                    Get all the bears.
/api/bears	          POST	                  Create a bear.
/api/bears/:bear_id	  GET	                    Get a single bear.
/api/bears/:bear_id	  PUT	                    Update a bear with new info.
/api/bears/:bear_id	  DELETE	                Delete a bear.
