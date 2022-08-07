# InstallReferrer Extension
Play Install Referrer Library (2.2)
* **
You can use the Google Play Store's Install Referrer API to securely retrieve referral content from Google Play. The Play Install Referrer API Client Library is written in the Java programming language and is a wrapper for the Android Interface Definition Language (AIDL) file that defines the interface to the Install Referrer service. You can use the Play Install Referrer API Client Library to simplify your development process.

This guide covers the basics of retrieving referral information from Google Play using the Play Install Referrer Library.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/aix.png"/>

## Start Connecton
* **
Before you can use the Play Install Referrer API Library, you must establish a connection to the Play Store app. Call the StartConnection to establish a connection to Google Play.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/start-connection.png"/>

## End Connection
* **
After getting referrer information, call the EndConnection to close the connection. Closing the connection will help you avoid leaks and performance problems.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/end-connection.png"/>

## Connected
* **
Connection established.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/connected.png"/>

## Disconnected
* **
Try to restart the connection on the next request to Google Play by calling the StartConnection method.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/disconnected.png"/>

## ConnectionError
* **
Read the message param to know about the error.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/connection-error.png"/>

## GetReferrerDetails
* **
After you have established a connection to the Play Store app, get the details from the install referrer.

**Caution:** The install referrer information will be available for 90 days and won't change unless the application is reinstalled. To avoid unnecessary API calls in your app, you should invoke the API only once during the first execution after install.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/get-referrer-details.png"/>

## GotReferrerDetails
* **
**referrerUrl:** The referrer URL of the installed package.
**referrerClickTime:** The timestamp in seconds when referrer click happens.
**appInstallTime:** The timestamp in seconds when installation begins.
**googlePlayInstant:** Boolean indicating if the user has interacted with the app's instant experience in the past 7 days.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/got-referrer-details.png"/>

## ReferrerDetailsFailed
* **
This event will be triggered when the extension failed to get referrer details.

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/referrer-failed.png"/>

## Extension specifications:
* **

<img src="https://raw.githubusercontent.com/jewelshkjony/InstallReferrer/main/images/download.png"/> <a href="https://github.com/jewelshkjony/InstallReferrer/releases/download/v2.2/com.jewel.installreferrer.aix">com.jewel.installreferrer.aix</a> (24.2 KB)
**SDK Version:** 2.2\
**Last amendment:** 07 August 2022
* **
