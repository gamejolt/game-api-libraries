= Postman Sandbox
This project includes a Postman collection and environment for testing Game Jolt API V1 calls.

== Getting Started
To use this project open or install Postman from the Google Chrome App Store. Now that Postman is running we need to import the project and environment.

=== Importing the Environment
In the top right of the screen is a drop down menu for selecting the Postman environment. Click this button and select Manage Environments. From the Manage Environments window select the Import option and click Choose Files. Select `Game%20Jolt%20Environment.postman_environment.json` from this folder and press Open. This will import an Environment titled "Game Jolt Environment". Select this environment and a list of the preset values will appear. A small amount of configuration is required before things are ready. You will need to update three of the Environment variables with values pertaining to the game you are working with. You must replace the values of `PrivateKey`, `username` and `user_token` with your Games API Private Key, Your Username and Your Token. Never commit these changes to source control! You may also want to update the GameId to the game you are working with.

Once this is complete, click the Update button in the bottom right of the window and then close the Manage Environments window. Your environment should now be properly configured. Huzzah!

=== Importing the Collection
Next we need to import the collection of api requests. To do this click Import from the top left of the main Postman window. Select Import File and click Choose Files. Find and select the `Game%20Jolt%20API.postman_collection.json` and click Open. A new folder will appear titled Game Jolt API. This new folder contains an organized set of API requests mirroring the available commands at http://gamejolt.com/api/doc/game. Select the command you would like to execute, modify the request parameters to fit your needs and click Send. Game Jolt's response will be shown in a console window below the request.

Note: Never remove the '{{signature}}' from the end of the request. This is automatically filled in by the pre-request scripts which will automatically generate a signature required for Game Jolt to accept the API request. Removing this will prevent any of these functions from working.