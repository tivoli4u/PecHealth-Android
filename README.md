<img
src="https://bluemixassets.eu-gb.mybluemix.net/api/Products/image/logos/conversation.svg?key=[starter-watson-conversation]&event=readme-image-view" alt="Watson Conversation Logo" width="200px"/>

## Conversation
Bluemix Mobile Starter for Conversation in Android

[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)
[![Platform](https://img.shields.io/badge/platform-android-lightgrey.svg?style=flat)](https://developer.android.com/index.html)

### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Conversation Configuration](#conversation)
* [Application Configuration](#configuration)
* [Run](#run)
* [License](#license)

### Summary
This Bluemix Mobile Starter will showcase the Conversation service from Watson and give you integration points for each of the Bluemix Mobile services.

### Requirements
* [Android Studio](https://developer.android.com/studio/index.html)
* A [Bluemix Account](https://www.bluemix.net/)

### Conversation Configuration
You will need to create or upload a conversation file to your Watson Conversation service (created for you) on Bluemix in order to allow interaction with the service.

In the dashboard of your Conversation service on Bluemix run the Conversation tooling dashboard by clicking the **Launch tool** button:

![ConversationDashboard](README_Images/ConversationDashboard.png)

Now create your own Conversation Workspace or import the sample workspace named `bluemix_mobile_qa_workspace.json` we have included in this project by selecting the import button from your Workspaces screen and navigating to the provided .json:
![ConversationImport](README_Images/ConversationImport.png)

After you have created or uploaded a Conversation Workspace you will need to get the Workspace Id. Click the **View details** list item to see the Workspace information. Save the **WorkspaceID** which we will need to include in our application configuration:

![ConversationWorkspace](README_Images/ConversationWorkspace.png)![ConversationWorkspaceID](README_Images/ConversationWorkspaceID.png)

### Application Configuration
* Open the project in Android Studio and perform a Gradle Sync.
* Navigate to `MainActivity.java` and input your Watson Conversation **WorkspaceID** you saved earlier in place of `YOUR_WORKSPACE_ID` on line ~260ish (look for the `doInBackground()` function in the `ConversationTask` class).

* Navigate to `MainActivity.java`, search for the `YOUR_WORKSPACE_ID` placeholder, and replace with the Watson Conversation workspaceID you saved or copied earlier.  The placeholder is found in the `ConversationTask` class, `doInBackground()` function.

### Run
You can now run the application on a simulator or physical device:

![ConversationRunningOne](README_Images/ConversationRunningOne.png)![ConversationRunningTwo](README_Images/ConversationRunningTwo.png)



The Watson Conversation service allows you to add a natural language interface to your application to automate interactions with your end users. This project shows an application of this service that allows you to have a conversation with Watson. Watson will send an initial conversation which you can then reply to and continue to interact with the service.

### License
This package contains code licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 and may also view the License in the LICENSE file within this package.
