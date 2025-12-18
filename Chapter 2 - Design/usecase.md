Actors

    Registered Member: A standard user interacting with the system.

    Registered Committee: A user with administrative privileges to manage content.

Use Cases by Actor

Registered Member

    Join Society: Enrolls the user in a specific society.

    Like Post: Allows the user to engage with content posted on the platform.

    Sync upcoming Society events to Calendar: Exports event data to the user's personal calendar.

Registered Committee

    Create Post: Publishes announcements or updates for members to view.

    Create Event: Schedules and publishes new society activities.

This Use Case diagram outlines the functional requirements for a society management system involving two distinct actors. Registered Members engage with the platform by joining societies, liking posts, and syncing upcoming events to their personal calendars. The Registered Committee holds administrative privileges, focusing on content generation by creating posts and scheduling new events for the society.



---------------


Member Calendar Synchronization

When a user clicks to sync, the system finds all future events in the database. It converts these records into a standard file format that personal calendars understand. The user then downloads this file to import the schedule into their own app.

Member Content Engagement

A user clicks the like button on a post. The system calculates the new total and saves the update in the database. The screen immediately refreshes to display the new number of likes.

Society Discovery and Enrolment

The system presents a list of active societies from the database. When a user selects a group to join, the system creates a formal link between the user and that society. This action instantly grants them member access.

Committee Content Publishing

Committee members use this tool to write posts. If the author links an event to the post, the system checks that the event actually exists. Once the check passes, the post is saved to the database.

Committee Event Management

A committee member enters event details like time and location. The system validates the information and saves it to the database. This action also triggers an update to the main calendar file so it remains accurate for future user downloads.
