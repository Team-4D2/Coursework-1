# Functional Requirements

 - The system should generate an ICS file for either a single event or a society's upcoming events (??), through data fetched from the database
 - The system should direct the user to their calander app of choice to save the event, or save the ICS file should no appropriate app be installed
 - The system should update to demonstrate to the user that the event was added

 - The system should query the database to return a list of attendees for an event

 - The system should update the database with a users RSVP (boolean, attending / not)
 - The system should update to demonstrate to the user their RSVP status 

 - The system should query the database to return a list of members within a society for users to view

 - The system should verify the target user is accepting friend requests
 - The system should update both users' outgoing/incoming requests, notifying target users of new requests

 - The system should notify a target user that they have been 'invited' to an event
 - The system should demonstrate to a user where an event they've been invited to is referenced, that they were invited to it by one or many friend users




## Michael 2# System Requirements

## Post Management

### Upload Post with Text/Images
- Users should be able to upload a post with a combination of text / images
  - The system should verify that all the text boxes are filled with valid data.
  - The system should send an API request to the backend with the verified data.
  - The system should then add this to the database via the database manager.

### Link Post to Event
- Users should be able to 'link' their post to an event
  - The system should fetch an event ID from the database using the restAPI.
  - The system should fetch a Post object from the database and then send a new request to the database manager inserting the eventURL to the posts row in the database.

## Event Management

### Create Event
- Users should be able to create an event
  - The system should verify that all event details are filled with valid data.
  - The system should send an API request to the backend with the verified event data.
  - The system should then add the new event record to the database via the database manager.

### Modify Event Details
- Users should be able to modify an event's details
  - The system should fetch the existing event object from the database using the restAPI to populate the fields.
  - The system should verify that the modified text boxes contain valid data.
  - The system should send an API request to the backend with the updated data and the event ID.
  - The system should update the specific event row in the database via the database manager.

### Switch Event Status
- Users should be able to switch an event's status (to public / private / scheduled)
  - The system should send an API request to the backend containing the event ID and the selected status tag.
  - The system should query the database manager to locate the specific event.
  - The system should update the status column for that event in the database to reflect the user's selection.

## Concern/Question Management

### Respond to Raised Concern
- Users should be able to respond to a raised concern/question
  - The system should fetch the ID of the raised concern from the database using the restAPI.
  - The system should verify that the response text box is filled with valid data.
  - The system should send an API request to the backend linking the new response to the concern's ID.
  - The system should insert the response text into the database via the database manager.


# Non-Functional Requirements

The system should not take more than 3 seconds to load the event dashboard.

The system should not take more than 3 seconds to complete the upload of a standard text post.

The system should be able to fetch and display a specific event's details within 3 seconds of the user's request.

The system will have login information saved, allowing logins to be reused (session persistence).

API requests should complete within 2-3 seconds under normal load

Maximum file size of 10MB per image

Users must be authenticated before creating, modifying, or linking posts/events

All input data must be sanitized to prevent SQL injection and XSS attacks
