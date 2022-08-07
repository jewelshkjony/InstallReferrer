# InstallReferrer - Play Install Referrer Library (2.2)
* **
You can use the Google Play Store's Install Referrer API to securely retrieve referral content from Google Play. The Play Install Referrer API Client Library is written in the Java programming language and is a wrapper for the Android Interface Definition Language (AIDL) file that defines the interface to the Install Referrer service. You can use the Play Install Referrer API Client Library to simplify your development process.

This guide covers the basics of retrieving referral information from Google Play using the Play Install Referrer Library.

![image|244x43](upload://5MmUqIrkFQhvFrDeHTgLKGFRYCF.png)

## Start Connecton
* **
Before you can use the Play Install Referrer API Library, you must establish a connection to the Play Store app. Call the StartConnection to establish a connection to Google Play.

![blocks|293x30](upload://opTAg1dJSgO2VepEUZ70sreoy1W.png)

## End Connection
* **
After getting referrer information, call the EndConnection to close the connection. Closing the connection will help you avoid leaks and performance problems.

![blocks (1)|288x30](upload://aG59jDywNm9Y4O69u9n73cxkgIf.png)

## Connected
* **
Connection established.

![blocks (2)|272x60](upload://t7E0dR3YOW7ZxPeXgdHnCDbbmiy.png)

## Disconnected
* **
Try to restart the connection on the next request to Google Play by calling the StartConnection method.

![blocks (3)|290x60](upload://wec2QL2WRMS6jsHQmpihLcPEBWf.png)

## ConnectionError
* **
Read the message param to know about the error.

![blocks (4)|308x85](upload://oWzOqUgtnNuKKqhIETw8DoMx2nD.png)

## GetReferrerDetails
* **
After you have established a connection to the Play Store app, get the details from the install referrer.

**Caution:** The install referrer information will be available for 90 days and won't change unless the application is reinstalled. To avoid unnecessary API calls in your app, you should invoke the API only once during the first execution after install.

![blocks (5)|310x30](upload://luogjctIGJ0U0rEAO1hxXCp1eEq.png)

## GotReferrerDetails
* **
**referrerUrl:** The referrer URL of the installed package.
**referrerClickTime:** The timestamp in seconds when referrer click happens.
**appInstallTime:** The timestamp in seconds when installation begins.
**googlePlayInstant:** Boolean indicating if the user has interacted with the app's instant experience in the past 7 days.

![blocks (6)|511x85](upload://hfN7oIpdanhEJpAwHGyDvByf05C.png)

## ReferrerDetailsFailed
* **
This event will be triggered when the extension failed to get referrer details.

![blocks (7)|339x85](upload://aWjmkpEjCklAE1rgLcGe1hzj6NX.png)
* **

## Extension specifications:
* **
[quote]
![download|16x16](upload://cmPsBKEwxbka0VANOKtqgIW8QSO.png) [com.jewel.installreferrer.aix|attachment](upload://dcPTQsG0pbME1qPlUAJEwagjVnJ.aix) (24.2 KB)
**SDK Version:** 2.2
**Last amendment:** 07 August 2022
[/quote]
* **
