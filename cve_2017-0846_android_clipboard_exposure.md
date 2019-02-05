# CVE-2017-0846 - Clipboard exposure on locked Android devices
<pre>
=========================================
- Exploit Title: An information disclosure vulnerability in the Android framework (clipboardservice)
- Version: Android versions 5.1.1, 6.0, 6.0.1, 7.0, 7.1.1, 7.1.2, 8.0 with Android Security Patches < January 2018
- Date: 2017-August-22
- Exploit Author: Andy Tyler (<a href="https://www.twitter.com/ticarpi">@ticarpi</a>)
- Website: <a href="https://www.ticarpi.com">https://www.ticarpi.com</a>
- Github: <a href="https://github.com/ticarpi">https://github.com/ticarpi</a>
- Tested on: Android 7.0, 7.1.1, 7.1.2
- Patched in: Android Security Patch => January 2018
- CVE: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-0846">CVE-2017-0846</a>
=========================================


I. DESCRIPTION
--------------
Sensitive Data Exposure from a locked Android Device via accessing the Clipboard functionality on the Lock Screen.

Exploitation allows a local attacker with physical access to a locked Android device to access any content currently stored on the Android Clipboard.
Such data may include passwords and other sensitive data.

II. PROOF OF CONCEPT
--------------------
It is possible to access the Clipboard contents by following these steps with physical access to a locked device:
[1] Await an incoming telephone call to the device.
[2] Swipe to send an SMS message in response.
[3] Choose to 'write your own...' message.
[4] Press and hold on the text input field and choose Paste to display the content of the Clipboard
[5] Optionally send the contents of the Clipboard to the number that is calling.

III. SOLUTION
-------------
Update (where possible) to a security patch level of January 2018 or newer.
</pre>
