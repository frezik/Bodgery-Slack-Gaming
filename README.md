# Bodgery-Slack-Gaming
A Slackbot for managing D&D character sheets, and allowing die rolls.

## Setup

1. Run "pip install -r requirements.txt" to install prereqs
2. Go to https://api.slack.com/apps?new_app=1 to create a new app
3. Add a 'Bots' feature type
4. Put in the name and display name
5. Go to "Basic Information" in the sidebar
6. Do "Install your app to your workspace"
7. Go to "OAuth Tokens"
8. Set the Bot User OAuth Token in your environment like:
   export SLACK_BOT_TOKEN=xxxXXxxXXxXXxXXXXxxxX.xXxxxXxxxx
7. Go back to "Basic Information" and find the "App Credentials" section
9. Set the Signing Secret in your environment like:
   export SLACK_SIGNING_SECRET=xxxxxxxxXxxXxxXxXXXxxXxxx
10. Set your assigned port number in your environment like:
    export SLACKBOT_EVENTS_PORT=xxxx
10. Put those environment commands into your .bashrc
11. Start your server with:
    python3 bot.py
12. Back in the Slack App Manager, go to the "Basic Information" page
13. Click "Add features and functionality", and add "Event Subscriptions"
14. Turn it on, and set the URL to:
    https://XXXX.shop.thebodgery.org/slack/events
    Replacing 'XXXX' with your assigned URL prefix
