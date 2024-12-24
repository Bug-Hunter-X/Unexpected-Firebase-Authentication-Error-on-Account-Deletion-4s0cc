# Unexpected Firebase Authentication Error on Account Deletion
This repository demonstrates an uncommon bug in Firebase Authentication where an unexpected error occurs if a user's account is deleted while the authentication process is underway. The bug is reproduced and a solution is proposed.
## Bug Description
The Firebase Authentication SDK may throw an unexpected error if the user's account is deleted or disabled during authentication.  This is due to the asynchronous nature of authentication operations, making it difficult to handle with standard error handling. 
## Reproduction
1. Clone this repository.
2. Install necessary dependencies: `npm install`
3. Run the application: `npm start`
4. Simulate account deletion while the authentication process is running (e.g., using Firebase console).