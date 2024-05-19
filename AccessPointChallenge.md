# Access Point Challenge Writeup

**SPOILER ALERT**

This is the solution for unlocking asteroids on your badge. Don't read further if you want to figure it out on your own.

---

After the badge powers up, it will wait between 30-60 minutes and then display the following on the screen:
```
Find me
jgadkds

m#gR9u4@
```

When this happens, the badge starts up it's WiFi Access Point. If you look at all the broadcasting SSIDs, you'll see at least one SSID that starts with **FreePublicWiFi-** and ends with the first code on the badge's screen. If you connect to that SSID using the second code for a password, you'll connect to the badge. It will assign you an IP in the 172.18.18.0/24 range.

From here, follow these steps:
* In your browser, if you enter **http://172.18.18.1**, you'll get to the badge's web app.
* The first thing to find is **/robots.txt**. In there you'll see that **/secret/** is disallowed.
* Next go to **/secret/**. Here you will see two files listed: **flag.txt** and **htpassword**. You need to log into the app to get to **flag.txt**, but you should be able to get **.htpassword**.
* If you download the contents of **.htpassword**, then you can run john against it to get the admin password. The password is very easily guessed.
* Once logged into the web app, if you load **flag.txt** and look at the source, you'll see a base64 value. Decode that value to get the flag.
* Go to **/submit** to submit the flag, this unlocks asteroids.

As a bonus, the JavaScript in the footer of every page pulls **/supersecret.json**, which contains a URL. The JavaScript outputs the json contents to the browser console. If you visited that URL during the conference, you would have been rickrolled and unlocked the related acheivement.
