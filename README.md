## [SQL Police Department](https://sqlpd.com/)
### Learn SQL while solving crimes :detective:
<br>

#### Case #1
"An illegal site's servers were seized in a recept operation. Please submit all users' details."
```SQL
SELECT * FROM USERS;
```
<br>

#### Case #2
"A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries' details."
```SQL
SELECT * FROM MAILING_LIST;
```
<br>

#### Case #3
"A hacked site subscribers’ details have surfaced on a darknet forum. Please submit all members mailing addresses and password hashes' details."
```SQL
SELECT MAILINGADDRESS, PASSWORDHASH FROM MEMBERS;
```
<br>

#### Case #4
"A hacked site subscribers' details have surfaced on a darknet forum. Please submit all subscribers subscribed since dates, password hashes and addresses' details."
```SQL
SELECT SUBSCRIBEDSINCE, PASSWORDHASH, ADDRESS FROM SUBSCRIBERS;
```
<br>

#### Case #5
"White hat hacker has sent SQLPD exposed members' details of a shady site connected to various persons of interest. Please submit all members addresses' details. Please make sure there are no duplicates."
```SQL
SELECT ADDRESS FROM MEMBERS GROUP BY ADDRESS;
```
<br>

#### Case #6
"White hat hacker has sent SQLPD exposed subscribers' details of a shady site connected to various persons of interest. Please submit all subscribers' details sorted by password hashes in ascending order."
```SQL
SELECT * FROM SUBSCRIBERS ORDER BY PASSWORDHASH;
```
<br>

#### Case #7
"A hacked site members' details have surfaced on a darknet forum. Please submit all members' details sorted by member since dates in descending order."
```SQL
SELECT * FROM MEMBERS ORDER BY MEMBERSINCE DESC;
```
<br>

#### Case #8
"A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries number of promotions sent, surnames and email addresses' details sorted by surnames in descending order. Please make sure there are no duplicates."
```SQL
SELECT DISTINCT PROMOTIONSSENT, SURNAME, EMAILADDRESS FROM MAILING_LIST ORDER BY SURNAME DESC;
```
<br>

#### Case #9
"An illegal site's servers were seized in a recent operation. Please submit all users access times and surnames' details sorted by access times in descending order and then by surnames in descending order."
```SQL
SELECT ACCESSTIME, SURNAME FROM USERS ORDER BY ACCESSTIME DESC, SURNAME DESC;
```
<br>

#### Case #10
"A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit the top 10 recerds' details when sorted by number of kids in ascending order and then by join dates in descending order."
```SQL
SELECT * FROM MAILING_LIST ORDER BY NUMBEROFKIDS, JOINED DESC LIMIT 10;
```
<br>

#### Case #11
"A hacked site subscribers' details have surfaced on a darknet forum. Please submit the top 10 subscribers surnames and full names' details when sorted by full names in descending order and then by usernames in ascending order. Please make sure there are no duplicates."
```SQL
SELECT DISTINCT USERNAME, FULLNAME FROM SUBSCRIBERS ORDER BY FULLNAME DESC, USERNAME LIMIT 10;
```
