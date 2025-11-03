---
theme: neversink
title: Cybersecurity - Best Practices
titleTemplate: '%s - VAW2025'
class: text-center
drawings:
  persist: false
transition: fade-out
mdc: true
fonts:
  sans: Roboto
  serif: Roboto Slab
  mono: Fira Code
layout: cover
color: rose-light
download: true
author: V.A.Karthik
favicon: /favicon.png
---

<div class="absolute top-10 right-10 text-right">
  <span class="font-500">
    V.A.Karthik, ACM/C&I <br/> 04-11-2025
	<Email v="karthik_va@nlcindia.in" />
  </span>
</div>

<div class="absolute bottom-10 right-10 text-right">
  <h1>Cybersecurity - Best Practices</h1>
  <p>Vigilance Awareness Week - 2025</p>
</div>

<!--
Good Morning!
CEO, CFO, GM/O&M, respected HODs, friends
How many of us write passwords on paper ?
-->

---
layout: quote
color: sky-light
quotesize: text-m
authorsize: text-s
author: 'Theme of VAW 2025'
---

सतर्कता: हमारी साझा जिम्मेदारी <br />
Vigilance: Our Shared Responsibility

<!--
Theme more apt to cybersecurity.
now a days more responsibility is expected from us 
-->
---
transition: slide-left
layout: top-title
align: l
color: blue-light
---

:: title ::

# Agenda

:: content ::

- Passwords and Management  
- DNS & DNS filtering   
- Spam & Scam
  - How to Identify ?
  - How to protect ourselves ?
- Privacy & Digital Wellbeing  

---
layout: section
color: cyan-light
---


# <mdi-form-textbox-password /> Passwords and Management 
<div v-click>
<hr>

- How Are We Managing Our Passwords ?
- How many online accounts we have ? 
- Are we re-using the same password ?

</div>
---
layout: side-title
side: l
color: cyan-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Passwords and Management

# <mdi-arrow-right />

:: content ::

## Password Statistics

- "123456" still top-used globally [(nordpass)](https://nordpass.com/most-common-passwords-list/)
- Average person has **100+ accounts** [(nordpass)](https://nordpass.com/blog/how-many-passwords-does-average-person-have/)
- 51% have their passwords memorized [(security.org)](https://www.security.org/digital-safety/password-manager-annual-report/)
- On average, people reuse the same password for at least four accounts [(forbes advisor)](https://www.forbes.com/advisor/business/software/american-password-habits/)

<!--
Satisfying ?
We are on the same boat
-->

---
layout: image-right
image: /password-01.jpg
class: neversink-cyan-light-scheme ns-c-bind-scheme
slide_info: false	
backgroundSize: contain
---

# Passwords and Management

# <mdi-arrow-right />

<br />

## How Passwords are Compromised

<br />

full infographic [here](https://www.ncsc.gov.uk/files/password_policy_infographic.pdf)


<!--
Explain each and protection against each of those
-->


---
layout: side-title
side: l
color: cyan-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Passwords and Management

# <mdi-arrow-right />

:: content ::

## Have I Been Pawned ? 

- Website: [https://haveibeenpwned.com](https://haveibeenpwned.com/)  
- Run by security researcher **Troy Hunt**  
- Database of compromised passwords
- Everyone is vulnerable to phishing - [Troy Hunt's Mailing list leak example](https://www.troyhunt.com/a-sneaky-phish-just-grabbed-my-mailchimp-mailing-list/)

<div class="absolute right-15 bottom-15">
<QRCode value="https://haveibeenpwned.com/" :size="200" render-as='svg'/>
</div>

---
layout: top-title-two-cols
side: l
color: cyan-light
---

:: title ::

# Passwords and Management

:: left ::

<div v-click> 

<Admonition type="important" title="Importance of Strong Passwords" color="teal-light">
- First line of defense in cybersecurity  <br/>
- Protects against unauthorized access <br/> 
- Weak passwords → quick compromise 
</Admonition>

</div>

<div v-click> 

## What Makes a Strong Password
  - Use longer passwords - Minimum 8 characters, However 15 is recommended  
  - Mix of upper/lowercase, numbers, symbols  
  - Avoid dictionary words / personal info  
  - Passphrases recommended `Enjoying-Unruffled-Doodle-Diligent` 
  - Use a [password generator](https://bitwarden.com/password-generator/#password-generator)
</div>  

:: right ::

<div v-click>
   
## How to Calculate Password Strength

- Length = exponential growth in difficulty  
- Example:  
  - 8-char lowercase → cracked in seconds  
  - 12-char with mix → years/centuries  
- Use [password strength checkers](https://bitwarden.com/password-strength/)

</div>
<div v-click>

<Admonition title="Edward Snowden on Passwords!" icon="mdi-lock-check">
In a 2015 interview with John Oliver, Snowden demonstrated how easy it is to crack a short password in a matter of seconds. To counter this, he suggested creating a much longer passphrase that is easier to remember but far more difficult for a computer to guess. 
His most famous example was `margaretthatcheris110%SEXY`. While this was used to illustrate a point, security experts warned against using any password that has been publicized. 
</Admonition>

</div>

---
layout: top-title-two-cols
side: l
color: cyan-light
---

:: title ::

# Passwords and Management

:: left ::

## Problem with Passwords

- Should be Unique for each website
- Impossible to remember
- Each Website Enforces different password policy and expiry

:: right ::
<div v-click> 

## Password Managers

- Securely Store, generate & autofill strong passwords  
- [Keepass](https://keepass.info/) (offline, open-source)  
- [Bitwarden](https://bitwarden.com/pricing/) (free, secure, sync across devices)


</div>

---
layout: side-title
side: l
color: cyan-light
titlewidth: is-3
align: rt-lt
---
:: title ::

# Passwords and Management

# <mdi-arrow-right />

:: content ::

# Demo - Bitwarden

<!--
Explain: Pricing, Sharing Feature, Passsword Generation Feature, URI, Autofill, Explain cons also
-->

---
layout: top-title-two-cols
side: l
color: cyan-light
---

:: title ::

# Multifactor Authentication

::left::

## 2FA

- SMS OTP (least secure)  
- Authenticator apps (Google Auth, Aegis, Authy)  
- Push notifications (Okta, Duo)

::right::

## Hardware Keys

- Uses FIDO2 standard
- Examples: **YubiKey, SoloKey**  
- Strong phishing-resistant authentication  
- Works with Bitwarden, Google, Microsoft, GitHub, etc.

---
layout: section
title: Demo - Hardware Keys
color: cyan-light
---

# Demo - 2FA & Hardware Keys

- Recommended TOTP App: [Ente Auth](https://ente.io/auth/) - FOSS, Sync across devices, No lockin
- Recommended MFA App: [Duo](https://duo.com/)
- Checkout [2fa.directory](https://2fa.directory/in/) website for the services that support various MFA methods

<!--
Explain: No. of keys required, what if keys were lost 
-->
---
layout: side-title
side: l
color: cyan-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Passwords and Management

# <mdi-arrow-right />

:: content ::

## Backup Codes

<AdmonitionType type="caution">
Losing access to your two-factor authentication (2FA) method can lock you out of your accounts
</AdmonitionType>

- Always save backup codes when enabling 2FA  
- Store in a safe place (paper/secure vault)
- [Bitwarden security readiness kit](https://bitwarden.com/resources/bitwarden-security-readiness-kit/)

<img src="/backup-codes.jpg" alt="alt text" width="300"/>

<!--
Basically one needs proper passwor manager setup and recovery code for password manager written down.
In addition backup of password used for 2FA app.
-->
---
layout: side-title
side: l
color: cyan-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Passwords and Management

# <mdi-arrow-right />

:: content ::

## Passkeys

<AdmonitionType type="info" title="" color="teal-light">
  Passkeys offer a way of confirming you are who you say you are without remembering a long, complicated password, and in a manner that's resistant to common attacks on passwords like phishing and dictionary attacks.
</AdmonitionType>

- Next-gen passwordless authentication  
- Uses device biometrics (fingerprint, FaceID)  
- Backed by Google, Apple, Microsoft
- You an save your generated passkeys in password managers
- [passkeys.directory](https://passkeys.directory/)


<!--
Use passkeys as password replacement. Better to have second factor setup.
-->
---
layout: section
color: emerald-light
---


# <mdi-dns /> DNS - Domain Name System

<hr>
<div v-click>
<img src="/dns.gif" />

</div>

---
layout: top-title-two-cols
side: l
color: emerald-light
---

:: title ::

# DNS

::left::
<div v-click>

## What is DNS

- Domain Name System = Internet’s Phonebook  
- Converts names (google.com) → IP addresses
</div>
::right::
<div v-click>

## How DNS Works

- User enters website URL  
- Request sent to DNS resolver  
- Resolver queries authoritative servers  
- IP address returned → browser connects
</div>
---
layout: full
color: emerald-light
---

<img src="/dns.svg" />

---
layout: top-title-two-cols
side: l
color: emerald-light
---

:: title ::

# DNS -> Cybersecurity

::left::

<div v-click>

## Why DNS Is Critical in Modern Cybersecurity

- It’s the first step in almost every internet connection.
- It’s often unmonitored or unencrypted, making it easy to exploit.
- It can be used to deliver, command, or conceal malware.
- DNS logs provide early warning signs of infection, compromise, or abuse.

In short, if you control or monitor DNS, you can prevent, detect, or disrupt many cyberattacks before they succeed. <a href="https://controld.com/blog/what-is-dns-cybersecurity/"><mdi-open-in-new /></a>

</div>

::right::

<div v-click>

## Core DNS Security Tools You Should Use

- DNSSEC (DNS Security Extensions)  
- Encrypted DNS (DoH and DoT)
- Real-Time DNS Analytics
- **DNS Filtering**

</div>
---
layout: top-title-two-cols
side: l
color: emerald-light
---

:: title ::

# DNS Filtering

::left::
<div v-click>

## How DNS filtering works

- A user requests a domain (e.g., badsite.com).
- The DNS filtering service checks that domain against threat categories or allow/block lists.
- If the domain is flagged (malware, phishing, etc.), the request is blocked.
- If it’s clean, the DNS query proceeds normally.

</div>

::right::
<div v-click>

## Using Free DNS filtering service

- [controld.com](https://controld.com/free-dns)
- [recommended DNS providers](https://www.privacyguides.org/en/dns/#recommended-providers)
- **Paid:** NextDNS, ControlD

## NextDNS Features

- Blocks ads & trackers  
- Parental controls (safe search, category filters)  
- Privacy
</div>
---
layout: side-title
side: l
color: emerald-light
titlewidth: is-3
align: rt-lt
---
:: title ::

# DNS

# <mdi-arrow-right />

:: content ::

# Demo - NextDNS

<!--
- Pricing, Family option, block NRD 
- Some services just work, nextdns is one
-->

---
layout: section
color: amber-light
---

# <mdi-phone-cancel /> Spams & Scams

<hr>

<div v-click>
<img src="/scam.jpg" width="300px"/>
</div>

---
layout: top-title-two-cols
side: l
color: amber-light
---

:: title ::

# Fighting Spams and Scams 

::left::
<div v-click>

## Spam

Spam refers to unwanted messages sent in large numbers through email, texts, or social media

- Marketing spam
- Social media spam
- SMS spam
- Robocall spam
</div>
::right::
<div v-click>

## Scam

A scam is a scheme meant to cheat people or businesses out of money or personal information

- Phishing scams
- Identity theft scams
- Investment scams
- Fake lottery scams
- Tech support scams
- AI impersonation scams
</div>
---
layout: top-title
side: l
color: amber-light
---

:: title ::

# Identify Scam / Spam / Phishing 

:: content ::

- Check sender email / phone number  
- Hover over URLs → look for mismatches  
- Spelling errors, urgent tone
- Unrealistic promises
- Unsolicited offers
- Threats and pressure
- Suspicious attachment

<SpeechBubble position="l" animation="float" shape="round" maxWidth="600px" v-drag="[461,63,400,160]">
Congratulations, ! You’ve won a grand prize of $250,000 in our International Lottery Draw. To claim your prize, reply with “CLAIM” and your full name and address
</SpeechBubble>

<SpeechBubble position="l" animation="float" shape="round" maxWidth="600px" v-drag="[461,240,400,200]">
Hi, this is Chris from Microsoft Support. We've detected a critical virus on your computer. To prevent permanent data loss, we need to connect to your computer remotely to fix it. You'll need to provide your account information first
</SpeechBubble>


---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - Identity Theft

:: content ::

Identity theft is the act of wrongfully obtaining someone’s personal information (that defines one’s identity) without their permission. The personal information may include their name, phone number, address, bank account number, Aadhaar number or credit/debit card number etc.

- **Do not close the browser window without logging out of the account.**
- Do not save your username and password in the web browser
- Permanently delete all documents downloaded on public computers.
- Never provide details or copy of identity proofs (e.g. PAN Card, Aadhaar Card, Voter Card, Driving License, Address Proof) to unknown person/organization.
- Do not share sensitive personal information (like Date of Birth, Birth Place, Family Details, Address, Phone Number) on public platforms.
- Always ensure that credit/debit card swipes at shopping malls, petrol pumps, etc. are done in your presence. Do not allow the sales person to take your card away to swipe for the transaction (to avoid card skimming)

---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - Social Engineering

:: content ::

Attackers play with the minds of the user to trap them with lucrative
offers. Once trapped, the attackers can exploit the victim by either stealing money or stealing sensitive personal information (name, Aadhaar details, bank account details etc.) or harm the victim in any other way. The entire basis of this kind of attack is to make the victim fall into their trap by sending fake e-mails, calls or SMSs

- Always verify the correctness of the domain of the e-mail ID, for example, all government websites have “.gov.in” or “.nic.in” as part of their web address.
- Do not respond to messages from unknown source requesting personal or financial details even if it assures credit of money into your bank account.
- Do not get petrified if you receive a call stating that your card is blocked. Bank will never convey such information on call.
- **Do not share your PIN, password, card number, CVV number, OTP etc. with any stranger, even if he/she claims to be bank employee. Bank will never ask for any vital information.**
- Keep your bank’s customer care number handy so that you can report any suspicious or un-authorized transactions on your account immediately.

---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - Social Media Frauds 

:: content ::

Social Media has become an integral part of our lives. One can understand the entire history of an individual through their social media profile and can even predict future events based on patterns in the past. This poses a threat to an individual as unwanted access to social media profile can cause loss of information, defamation or even worse consequences such as physical/sexual assault, robbery etc. Hence, protection and appropriate use of social media profile is very important.

- Do not accept friend requests from strangers on social networking sites 
- Restrict access to your profile. Social media sites offer privacy settings for you to manage who can view your posts, photos, send you friend request etc.
- Ensure your personal information, photos and videos are accessible only to your trusted ones.
- Discuss safe internet practices with your friends and family regularly.
- Monitor your kid’s activity on internet/social media. Enable parental controls on
computer/mobile devices.

<!--
- Be careful :
 -- If your child’s behavior is changing and he/she is more aggressive than
 before.
 -- If suddenly your child stops talking with you or his/her friends.
 --If he/she stops using digital devices or is scared.
- Make your children aware that cyber bullying is a punishable crime so that
neither do they indulge themselves in cyber bullying nor do they let anyone
tease them.
- Even if the children or students know about any friend who is a victim of cyber
bullying, they should help the victim. Report the matter to parents or teachers
immediately.
- Do not delete offensive messages as it will help the police in investigation.
-->

---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - Mobile App Frauds 

:: content ::

Mobile applications are widely used not only for entertainment but also for ease and convenience to perform day-to-day tasks such as bill payments, bank accounts management, service delivery etc. As a result, these applications are more prone to cyber-attacks

- **Always install mobile applications from official application stores or trusted sources**.
- Scrutinize all permission requests thoroughly, especially those involving privileged access, when installing/using mobile applications. For example, a photo application may not need microphone access.
- Regularly update software and mobile applications to ensure there are no security gaps.

<!--
use virustotal for scanning mobile apps
-->
---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - Online Banking Frauds 

:: content ::

As all the banking services are shifting towards online platforms, cyber frauds related to banking are also increasing.

- Register your personal phone number and e-mail with your bank and subscribe to notifications. These notifications will quickly alert you on any transaction and the unsuccessful login attempts to your net-banking account.
- Always review transaction alert received on your registered mobile number and reconcile with the amount of your purchase.
- Do not save your usernames and passwords in the web browser. Use Password Managers!
- Always be sure about the correct address of the bank website and look for the ‘‘lock’’ icon on the browser’s status bar while visiting your bank’s website or conducting an online transaction. Always be sure ‘‘https’’ appears in the website’s address bar before making an online transaction. The ‘‘s’’ stands for ‘‘secure’’ and indicates that the communication with the webpage is encrypted.
- **Disable international transaction option on your credit card & enforce per transaction limits**

<!--
show a demo in imobile app
-->

---
layout: top-title
side: l
color: amber-light
---

:: title ::

# How to protect yourself - General

:: content ::

- Always download software or applications from known trusted sources only. **Never use pirated software on your systems/devices.**
- Always change the default admin password on your Wi-Fi router to a strong password known only to you. In addition, always configure your wireless network to use the latest encryption.
- Be cautions while browsing through a public Wi-Fi and avoid logging in to personal &
professional accounts such as e-mail or banking on these networks. 
- Always use virtual keyboard to access net-banking facility from public computers; and logout from banking portal/website after completion of online transaction.
- **Note the IMEI code of your cell phone and keep it in a safe place. The operator can blacklist /block / trace a phone using the IMEI code, in case the cell phone is stolen.**
- **Discuss safe internet practices with your friends and family regularly! Motivate them to learn more about cybercrimes and safe cyber practices.**
- **Do not store unencrypted data on cloud services**

<!--

- Do not post photos which contain exif information
- UPI PIN is not needed while receiving payments

Doosra Number
- Virtual number service for registrations  
- Protects primary number from spam

Fake Data
- Don’t share real DOB / name everywhere  
- Use fake info for non-critical signups

Aadhar Virtual Number
- Use Virtual ID (VID) instead of Aadhaar number
-->

---
layout: top-title
side: l
color: amber-light
---

:: title ::

# Cybercrime Reporting

:: content ::

- ☎️ Dial **1930** for fraud & cybercrime help
- 🌐 National Cyber Crime Reporting Portal - [cybercrime.gov.in](https://cybercrime.gov.in)  
- To report lost or stolen mobile phones, file a First Information Report (FIR) with the police. Post filing the FIR, inform Department of Telecommunications (DoT) through the helpline number 14422 or file an online compliant on Central Equipment Identity Register (CEIR) portal by visiting https://ceir.gov.in. After verification, DoT will blacklist the phone, blocking it from further use. In addition to this, if anyone tries to use the device using a different SIM card, the service provider will identify the new user and inform the police.

## Government Apps

- **Sancharsathi** (report spam SMS/calls, check registered mobile nos. on your name)  
- **TRAI DND** registry (check an register for DND)

---
layout: section
color: teal-light
---

# <mdi-shield-lock-outline /> Privacy & Digital Wellbeing

<hr>

<!--
Privacy is the ability of an individual or group to seclude themselves or information about themselves, and thereby express themselves selectively
-->
---
layout: quote
color: teal-light
quotesize: text-m
authorsize: text-m
author: Edward Snowden
---

Arguing that you don't care about privacy because you have nothing to hide is like saying you don't care about free speech because you have nothing to say

---
layout: top-title-two-cols
side: l
color: teal-light
---

::title::

# Data - The New Oil

::left::

<div v-click>

## How Big Tech Collects Your Data

- Web Browsing & Search History
- Social Media Activity
- Smartphone Apps & Permissions
- Voice Assistants & Smart Devices
- Purchases & Online Shopping
- Location Tracking
- Emails & Cloud Storage

</div>

::right::

<div v-click>

## How Big Tech Uses Data

- Targeted Advertising 
- Product & Service Improvement
- Profiling & prediction  
- Selling to data brokers


<AdmonitionType type="warning" title="">
  Android Manifest <a href="https://peabee.substack.com/p/everyone-knows-what-apps-you-use">example</a>
</AdmonitionType>

<AdmonitionType type="info" title="" color="teal-light">
  Watch the documentry 'The Social Dilemma'
</AdmonitionType>

</div>
---
layout: top-title-two-cols
side: l
color: teal-light
---

::title::

# How to Protect Your Privacy Online

::left::
<div v-click>

- Block ad and trackers using DNS filtering 
- Use VPN
- Prefer Web Apps
- Disable Location Services When Not Needed 
- Limit App Permissions
- Use Encrypted Messaging & Email Services
- [Read TOS](https://tosdr.org/en/)

</div>

::right::
<div v-click>

## Social Media Alternatives
- **Fediverse** (Mastodon, Lemmy, Pixelfed)

## 💬 Chat Alternatives
- Signal, Matrix

## More Here 👇
🌐 [privacyguides.org](https://privacyguides.org)
</div>
<!--
The Fediverse is a collection of interconnected social media platforms that can communicate with each other using a common protocol called ActivityPub
-->

---
layout: side-title
side: l
color: teal-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Digital Wellbeing

# <mdi-arrow-right />

:: content ::
<div v-click>

## It's OK to be Bored 😒 <a href="https://www.youtube.com/watch?v=orQKfIXMiA8"><mdi-open-in-new /></a>
- Constant stimulation = digital fatigue  
- Allow downtime for mental health
</div>
<div v-click>

## 📝 Some Tips
- Turn Off Notifications
- Keep Mobile Phone Out of Reach
- Limit Screen Time
</div>
<!--
Life changing descions are taken in travel / shower <br/>
Brain thinks about deep quesions during boredom  <br/>
FOMO  <br/>
-->
---
layout: section
title: Demo - Password Manager
color: cyan-light
---

# Key Takeaways

- Use Password manager
- Compulsarily use one form of 2FA - TOTP << Duo << Hardware Keys
- Keep MFA recovery codes safe
- Use DNS filtering service 
- Mind your privacy
- Turn off Notifications
- Stay Updated

---
layout: section
title: Interesting Links
color: slate
---

# Interesting Links

- 🎧 [Darknet Diaries podcast](https://darknetdiaries.com/)  
- 🌐 [Privacyguides.org](https://privacyguides.org)
- [IntelTechniques](https://inteltechniques.com/)  
- 💌 [Proton.me](https://proton.me) (Mail, Drive, VPN)
- Reddit: [r/privacy](https://reddit.com/r/privacy), [r/selfhosted](https://reddit.com/r/selfhosted), [r/degoogle](https://reddit.com/r/degoogle)
- [Cyberawareness](https://cybercrime.gov.in/Webform/CyberAware.aspx)
- 🔎 [VirusTotal](https://www.virustotal.com/gui/home/upload)

---
layout: side-title
side: l
color: indigo-light
titlewidth: is-3
align: rt-lt
---

:: title ::

# Any Questions ? <a href="https://m.xkcd.com/1256/" class="text-s"><mdi-open-in-new /></a>

:: content ::
 
<img src="/questions.png" width="600px" />

---
layout: section
title: Thank You
color: indigo-light
---

# Thank You!
<hr />
Stay Vigilant, Stay Secure 🔒

<div class="absolute right-15 bottom-15">
<QRCode value="http://vakarthik.github.io/vaw2025/" :size="150" render-as='svg'/>
</div>
