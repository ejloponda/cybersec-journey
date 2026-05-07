# 🌐 Walking An Application — Page Source Viewing
**Platform:** TryHackMe  
**Path:** Jr Penetration Tester → Web Hacking  
**Status:** ✅ Completed 
__________
## 🎯 Objective
Learn how to manually review a web application for vulnerabilities 
using only a browser's built-in developer tools.

__________

## 🧠 Key Concepts Learned
- Page source is the human-readable code returned by the web server
- Page source is made up of HTML, CSS, and JavaScript
- Viewing page source can reveal hidden comments, credentials, 
  and hidden endpoints

___________
## 🎯 Target
**ACME Website** — used as the practice target for this room
_____________
![ACME WEBSITE](screenshots/ACME-WebPage.jpg) 

In this activity, We have four questions :

1. What is the flag from the HTML comment?
2. What is the flag from the secret link?
3. What is the directory listing flag?
4. What is the framework flag?

___________________
## ❓ Tasks & Solutions

### Task 1 — What is the flag from the HTML comment?

**Approach:**
- Opened page source in Google Chrome on Mac (`Cmd + U`)
- Searched for HTML comments using `Cmd + F` and typing `<!--`
- Found a clue left in the comment section
- Manually Adding the suspected directory to the URL

![Viewing Page Source](screenshots/02_Viewing_PageSource.png)
![Clue from Comments](screenshots/03_clue_from_comments.png)
![Adding New Home Beta URL](screenshots/04_adding_newhomebeta_url.png)
![Flag # 1](screenshots/05_Question1_Flag.png)

**Flag 1:** `THM{REDACTED}` ✅

--------------------------

### Task 2 — What is the flag from the secret link?

**Approach:**
- Searched for the word "secret" via `Cmd + F` 
- Found a match and clicking it

![Viewing secret-page via Page Source](screenshots/08_Searching_for_secret.png) 

![Flag # 2](screenshots/09_Flag2.png)

**Flag 2:** `THM{REDACTED}` ✅


### Task 3 — What is the directory listing flag??

**Approach:**
- Inspect the webpage via inspection tool
- Discovered "assets" folder via sources tab
- Manually adding "assets" to the URL
- Discovered different files including flag.txt
- clicking flag.txt


**Flag 3:** `THM{REDACTED}` ✅


