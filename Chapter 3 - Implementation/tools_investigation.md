We will be running the backend using Python with the Flask framework alongside JWT and Flask-SQLAlchemy. Flask allows us to quickly and easily set up multiple web endpoints. JWT will provide access control for the Flutter mobile app. The Flutter authorization tokens will be created on the Flutter app and sent in the URL request to Flask.

After the request endpoint has verified that the JWT is valid, it can make a request to the SQL database using SQLAlchemy, extract the relevant data, and return it via a REST API. The entire server will be run within a Docker container so it can be easily deployed onto a VM or VPS.

The frontend will be developed entirely in Flutter, with a form of persistent storage to keep the user logged in using the Flutter shared storage system. When the app opens, a JWT will be created for this session. Once this has been done, the app will download the list of users' societies from the server's backend and check for new notifications
