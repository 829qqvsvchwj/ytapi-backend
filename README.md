# ytapi-backend

This routes YouTube videos through heroku to provide a YouTube API that users can access without accessing googlevideo or YouTube servers.

## Prerequisites

Get a YouTube Data API Key (avalible from Google Cloud Portal)

## Automatic Setup Process (recommended)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Manual Setup Process

1. Fork this repository. Make sure your branch is up-to-date with master.
2. Now, go to https://heroku.com and create an account (or log in, if you already have an account).
3. On your dashboard, click on "New" -> "Create new app"
4. Give your app a name (referred to as __{YOUR_APP_NAME}__) and select a region for deployment.
5. Go to the __Deploy__ section on your new app's dashboard.
    1. Under `Deployment Method`, select the GitHub option. You should be prompted to authorize Heroku's usage of your GitHub account information.
    2. Under `Connect to GitHub`, make sure your account is selected and type in "dmhacker-youtube" for the repository to search for.
    3. If you correctly forked this repository and typed in the repository name correctly, this should show up as an option to connect to. Click on "Connect".
6. Now, go to the __Settings__ section on your app's dashboard.
    1. Under `Config Variables`, click on "Reveal Config Vars" and then enter in the following key-value pair(s):

        | Key                  | Value                                                                 |
        | -------------------- | --------------------------------------------------------------------- |
        | YOUTUBE_API_KEY      | the YouTube API key you generated earlier                             |

    2. Next, under `Buildpacks`, click on "Add buildpack" and click on the icon named "nodejs".
7. Now, you're ready to deploy! Go back to the __Deploy__ section.
    1. Under `Manual Deploy`, click on "Deploy Branch".
8. If you get a "Your app was successfully deployed", congratulations, you are done, and your app should be running!
9. To verify, open up https://__{YOUR_APP_NAME}__.herokuapp.com in a new tab and see if it returns a correctly formed landing page.

## Special thanks
Thanks to David Hacker, who created the code this API is based off of.
Original code used under MIT License (www.github.com/dmhacker/dmhacker-youtube)
