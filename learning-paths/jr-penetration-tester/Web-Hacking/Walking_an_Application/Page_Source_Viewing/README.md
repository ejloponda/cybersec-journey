The page source is the human-readable code returned to our browser/client from the web server each time we make a request.

The returned code is made up of HTML ( HyperText Markup Language), CSS ( Cascading Style Sheets ) and JavaScript, and it's what tells our browser what content to display, how to show it and adds an element of interactivity with JavaScript.

For this purposes, viewing the page source can help us discover more information about the web application.

[ACME WEBSITE](screenshots/ACME-WebPage.jpg) --> The Target website 

In this activity, We have four questions :

1. What is the flag from the HTML comment?
2. What is the flag from the secret link?
3. What is the directory listing flag?
4. What is the framework flag?

For number 1

This is what I did :

[Viewing Page Source](screenshots/02_Viewing_PageSource.png) | Check for clues; for this I was using Google Chrome on a Mac

[Clue from comments](screenshots/03_clue_from_comments.png) | Clue was left on the comment section

[Inserting suspected directory to the URL](screenshots/04_adding_newhomebeta_url.png) | adding "/new-home-beta" to the url

[Flag # 1](screenshots/05_Question1_Flag.png)


For number 2

[Viewing secret-page via Page Source](screenshots/06_secret-page.png) | Via Page Source inspection, there is a secret-page link that you can click

[Flag # 2](screenshots/07_Flag2.png)



