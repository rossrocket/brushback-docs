# Setting Up AMQ Test Environment
This guide provides instructions for setting up and testing the AMQ environment in a controlled manner.
To enable test mode, you’ll configure the settings to use the testing environment, reconnect ActiveMQ,
and load the available test game. For testing AMQ data without loading a game,
specific settings must be adjusted, including entering the test venue ID and reconnecting.

Following these steps ensures that Brushback subscribes to the correct topics for testing purposes.

## Enabling Test Mode
1. Go to the "Settings" tab
2. Check "Use testing environment"
3. At the bottom of the "Settings" page, click "Save & Apply"
4. Under "ActiveMQ Settings", click "Disconnect then Reconnect"
5. Go to the "Load Game" tab, and select the game you want to load
    - Currently, there is only one test game to use

## Testing only AMQ
If you want to only want to test AMQ data, then you do not need to load a game.

1. Go to the "Settings" tab
2. Ensure "Only send matching Game PK" is ☐ unchecked 
3. Ensure "Override Venue ID" is ☑ checked
4. Enter in the ID for the test venue
    - Currently, there is only one test venue `4249` (Salt River Field at Talking Stick)
6. Click "Save Changes"
7. Click "Disconnect then Reconnect"

Brushback will now be subscribed to topics from the given venue ID

## Appendix
![image](https://github.com/user-attachments/assets/efb45563-e68c-4856-954f-46cc0268efd0)
