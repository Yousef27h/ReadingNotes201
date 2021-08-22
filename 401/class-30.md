# Cognito

The Amplify Framework uses Amazon Cognito as the main authentication provider. Amazon Cognito is a robust user directory service that handles user registration, authentication, account recovery & other operations. It provides the necessary authorization to the other Amplify categories.

To add authentication to our app project, we use this command first `amplify add auth`

After completing it `amplifyconfiguration.json` should be updated. Then we just add dependencies to our app's `build.gradle` to start using authentication in our app.

The Auth category enables the user to register, confirm attributes like email/phone, and sign in with optional multi-factor authentication. It is set up to use Amazon Cognito User Pools which manages the users and their properties.



