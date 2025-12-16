The non-functional requirements will be tests by several methods, including timing, and testing inputs. 

  

Non-functional requirements 1, 2, 3 and 5 will be tested by timing the speed of the system, passing if they do not exceed the time limit 

requirement 4 will be tested by simulating logging in and ending the session then begining another, if the user is still logged in the test passes 

requirement 6 will be tested by trying to upload an image over the max file size, if it fails the test passes 

requirement 7 will be tested by trying to mutate a post while unauthenticated, if the system does not allow the mutation the test passes 

requirement 8 will be tested by trying to execute XSS/SQL injection attacks if the attacks fail the test passes 

  

the tests will be automatically run via flutter unit tests; other testing methods would be harder to integrate into the system as we are already using flutter, and as it’s the front end of the system, the other components can be tested through it. 