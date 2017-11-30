# Upload and sharing files in Google Drive using API v3

This example is based in [Google Drive API Java Quickstart Guide](https://developers.google.com/drive/v3/web/quickstart/java)

## Prerequisites

To run this example, you'll need:

* Java 1.7 or greater.
* Gradle 2.3 or greater.
* Access to the internet and a web browser.
* A Google account with Google Drive enabled.

##  Step 1: Turn on the Drive API

1. Use this [wizard](https://console.developers.google.com/start/api?id=drive) to create or select a project in the Google Developers Console and automatically turn on the API. Click **Continue**, then **Go to credentials**.
2. On the **Add credentials to your project** page, click the **Cancel** button.
3. At the top of the page, select the **OAuth consent screen** tab. Select an **Email address**, enter a **Product name** if not already set, and click the **Save** button.
4. Select the **Credentials** tab, click the **Create credentials** button and select **OAuth client ID**.
5. Select the application type **Other**, enter the name "Drive API Java Sample", and click the **Create** button.
6. Click **OK** to dismiss the resulting dialog.
7. Click the **Download JSON** button to the right of the client ID.
8. Rename this file to `client_secret.json`.

## Step 2: Set up the sample

1. Clone this repository using `git clone` to a folder in your computer.
2. Move the `client_secret.json` file you downloaded in Step 1 into the `src/main/resources/` directory of the project.
3. Copy the `.pdf` files that you want upload and sharing in Google Drive, into the `files` directory of the project.

## Step 3: Run the sample

1. Open a terminal on your computer and go to project's directory.
2. Build and run the sample with the command: `gradle -q run`.

The first time you run the sample, it will prompt you to authorize access:

* The sample will attempt to open a new window or tab in your default browser. If this fails, copy the URL from the console and manually open it in your browser. 
* If you are not already logged into your Google account, you will be prompted to log in. If you are logged into multiple Google accounts, you will be asked to select one account to use for the authorization.
* Click the **Accept** button.
* The sample will proceed automatically, and you may close the window/tab.
