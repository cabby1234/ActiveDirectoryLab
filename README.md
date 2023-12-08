<h1>Hacking WPA/WPA2</h1>

<h2>Description</h2>
OWASP Juice Shop is a project that serves as a great platform for testing web application security. It incorporates a wide range of security vulnerabilities inspired by real-world scenarios, making it an ideal playground for penetration testers. The application is built on modern web technologies and includes challenges that cover aspects such as injection attacks, cross-site scripting (XSS), broken authentication, and more. I have highlighted a few of the vulnerabilites I exploited in the slideshow; along with my overall experience working through Juice Shop.
<br />

<h2>Tools Used</h2>

- <b>Aircrack-ng</b> 
- <b>Wireshark</b>

<h2>Environments Used </h2>

- <b>Kali Linux virtual machine ran on VMware.</b>

<h2>Lab walk-through:</h2>

<p align="center">
<strong>Kill processes and put our WIFI interface in monitor mode:</strong>
 <br/>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/43d47054-3cf3-46a5-9742-29b7ee584f17">
<br>
<br>
 <br>
<strong>Perform our reconaissance on the target and capture the WPA handshake, deauthenticate if needed:</strong>
 <br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/de076149-e800-4c3c-9138-876a1df4bf30">
<br>
<br>
<br>
<strong>The capture of our WPA handshake pulled up in Wireshark:</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/bb486f75-80e9-466b-afb4-bba0030f9206">
<br>
<br>
 <br>
<strong>Aircrack-ng command to obtain the wireless keys, using the rockyou.txt wordlist:</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/0a4f0847-8700-46ac-bb0e-047f1191e6f7">
<br>
<br>
 <br>
<strong>After running the command we were able to obtain the keys in seconds. (Keys are blocked out to maintain lab integrity)</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/9a7ff105-3b76-4ec3-97ae-c80ec7cb94fc">




<!--
 ```diff
- text in red
+ text in green
! text in orange
@@ text in purple (and bold)@@
```
--!>
