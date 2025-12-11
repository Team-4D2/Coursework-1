## early/draft System requirments
- user-account have: Societies, email
- Societies have Calenders, committee-members, Posts, notfication-perms
- Posts have: text, images, videos, descriptions
- Societies can send notifcations, export calenders, make posts
- Calenders have: events,
- Events have: date, time, catogories, description, location, length
- committee-members have: email, name
 
- Societies can only send notfications if the user-account allows it to
- Societies calender can be empty
- Societies can have no posts
- Societies have to have committee members

- user-account can subscribe to societies
- user-account have to have a valid portsmouth uni email address

- posts have to have minimum one of the following: text, image, video

## nickyyl from user_requirements.md

- users should be able to add a single societies' event to their device calander
- users should be able to add all a socities event's to their device calander
 - The system should generate an ICS file for either a single event or a society's upcoming events (??), through data fetched from the database
 - The system should direct the user to their calander app of choice to save the event, or save the ICS file should no appropriate app be installed
 - The system should update to demonstrate to the user that the event was added

- users should be able to view a guest list
 - The system should query the database to return a list of attendees for an event

- users should be able to RSVP to an event
 - The system should update the database with a users RSVP (boolean, attending / not)
 - The system should update to demonstrate to the user their RSVP status 
 
- users should be able to see a list of society members
 - The system should query the database to return a list of members within a society for users to view

- users should be able to add society members as their friends
 - The system should verify the target user is accepting friend requests
 - The system should update both users' outgoing/incoming requests, notifying target users of new requests

 - users should be able to 'invite' friends to a society event
 - users should be able to see distinctive features of an event they are invited to
  - The system should notify a target user that they have been 'invited' to an event
  - The system should demonstrate to a user where an event they've been invited to is referenced, that they were invited to it by one or many friend users
