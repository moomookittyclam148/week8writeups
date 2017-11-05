##GREEN WEBSITE

1. Username Enumeration
  - when trying to log in to the site when using a username that is in the database it shows the error Login was not successful in bold. When using a username that does not exist it shows the same error in normal text.

2. Cross-Site Scripting
  - In the contact part of the website, a user is allowed to insert a XSS script into the feedback part. When an admin or a user looks at the feedback page the script is ran.


##RED website

1. IDOR
  - Allows you to access a Salesperson who is not to be seen yet. Change id to equal 10 in url https://104.154.236.9/red/public/salesperson.php?id=10

2. CSRF
  - Allows users to submit a false form to the browser to change information in the database.
  use html file in /week8 folder for exploit.


##BLUE WEBSITE

1. SQLi
  - Can use a sql injection statement when looking for salespeople
  example https://104.154.236.9/blue/public/staff/salespeople/show.php?id=' OR SLEEP(10)=0--'

2. Session Hijacking/Fixation
  - Using two different browsers get the session id of a logged in user and copy it to the other web browser
