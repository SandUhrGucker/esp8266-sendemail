Send email with esp8266/Arduino, smtp auth and ssl support.

Examples:

ssl:<br>
  SendEmail e("mail.example.com", 465, "login", "password", 5000, true); <br>
  e.send("test@example.com", "me@example.com", "subject", "message"); <br>
  <br>
  
plain no auth:<br>
  SendEmail e("mail.example.com", 25, "", "", 5000, false);<br>
  e.send("test@example.com", "me@example.com", "subject", "message");<br>

(!) to debug the communication, uncomment line 4 in sendmail.h and add:
#define DEBUG_EMAIL_PORT Serial 

Info: today I spend much Time to connect to gamil.
At the End I give up. 
google doesnt want unconfirmed/unregisteres email-sender-clients without 2FA.
Just take an other smtp-provider.
