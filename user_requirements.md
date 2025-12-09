## User Requirements (Society Members):

## Lewis
- users should be able to log in / register
- users should be able to join multiple societies
- users should be able to contact a societies' committee
- users should be able toggle on/off notifications for a societies' feed
- users should be able to interact with posts
    - vote in polls
    - like
    - reply to the comittee

 ## Nickyyl
- users should be able to add a single societies' event to their device calander
- users should be able to add all a socities event's to their device calander
- users should be able to view a guest list
- users should be able to RSVP to an event
- users should be able to 'invite' friends to a society event = like a facebook poke
    - users should be able to add society members as their friends
        - users should be able to see a list of society members
    - users should be able to see distinctive features of an event they are invited to
    
## Michael

## User Requirements (Comittee Members, for their society):

- users should be able to upload a post with a combination of text / images
    - users should be able to 'link' their post to an event
- users should be able to manage events
    - create an event
    - modify an event's details
    - switch an event's status (to public / private / scheduled)
    - link a post
- users should be able to respond to a raised concern/question





## Michael 2
users should be able to upload a post with a combination of text / images
	The system should verify that all the text boxes are filled with valid data.
	The system should send a API request to the backend with the verified data.
	The system should then add this to the database via the data base manager.	

users should be able to 'link' their post to an event
	The system should fetch a event ID from the database using the restAPI
	The system should fetch a Post object from the database and then send a new request to the database manager inserting the eventURL to the posts row in the database.

Users should be able to create an event
    The system should verify that all event details are filled with valid data.
    The system should send an API request to the backend with the verified event data.
    The system should then add the new event record to the database via the database manager.

Users should be able to modify an event's details
    The system should fetch the existing event object from the database using the restAPI to populate the fields.
    The system should verify that the modified text boxes contain valid data.
    The system should send an API request to the backend with the updated data and the event ID.
    The system should update the specific event row in the database via the database manager.

Users should be able to switch an event's status (to public / private / scheduled)
    The system should send an API request to the backend containing the event ID and the selected status tag.
    The system should query the database manager to locate the specific event.
    The system should update the status column for that event in the database to reflect the user's selection.

Users should be able to respond to a raised concern/question
    The system should fetch the ID of the raised concern from the database using the restAPI.
    The system should verify that the response text box is filled with valid data.
    The system should send an API request to the backend linking the new response to the concern's ID.
    The system should insert the response text into the database via the database manager.
