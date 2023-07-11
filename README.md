## Sucre Web Application
This web application is a business inventory management system which displays purchase and sales report having keyed in the range of dates.
New products can be added as well which is used in altering the purchase form.

## Author:                                      Chidiebere Aginam 

## Links
https://www.sucremax.tech
https://www.linkedin.com/in/chidiebere-aginam-51b22b128
https://www.twitter.com/ChidiAginam
E-mail: chidiebereaginam@yahoo.com

## Installation:
After setting up a LAMP stack;
This application can be installed as follows:
On Ubuntu server preferably 20.04, navigate to /var/www/html folder. Or it can be customised to
a folder that contains a path to your domain name.
Deposit the files there, then log on to MYSQL
database and create a database named "ims480".
Exit from mysql and run the .sql file, there 
you go.

## Credential for admin panel
- username: admin
- Password: admin

## User Requirements:
1. Authentication for admin
2. Product Information Management (Add, Delete, Update)
   - Product Name
   - Product Description
   - Unit
   - Unit Price
3. Stock Management (Purchase and Sale)
4. Stock Status and Transaction Report (Daily and Monthly)

## Challenges:
Earlier, I stated in my proposal to use PHP language as a backend script, written some of the codes and ran them in my terminal, few of them worked. I tried to figure out what the problem was and after thorough scrutiny, I discovered that the files need API-like codes to relay information to the database.

As a result of this, I have been studious inorder to get the codes up and working as I never expected this occurrence. I chose to work with PHP because I thought it is compact and again had an architecture to bypass API configuration to save me the stress of having to route the webpages one after the other.

To solve this problem, I have recently reckoned on python language to see if I can generate codes for http request and response over Mysql database in my Ubuntu server.

Second week: I found it difficult connecting my web application to the SQL server but later found out why, I forgot that in my script, the password for establishing connection is 'root' whereas that in the server for root user without the sudo command never matched. Secondly, I logged into the database with a different user rather than the root.
Upon the discovery of this, I made adequate corrections and was able to log in using the following command:

alter user 'root'@'localhost' identified with mysql_native_password by 'root'

It wasn't easy making changes to my database. In the long run, I researched further so as to understand the dynamics of HTTP methods which helped me in making the web application interactive using the acronym CRUD which stands for: Create, Read, Update and Delete.


## Screen Shots
![admin login](https://user-images.githubusercontent.com/38730778/212720829-dc8a14dc-4125-49ec-9375-fba999fc5f1f.JPG)
![stock](https://user-images.githubusercontent.com/38730778/212720833-8b98b642-54ee-4eb1-a8ed-022d3552d853.JPG)
![purchase](https://user-images.githubusercontent.com/38730778/212720812-4926957c-a7aa-456e-a547-d04f8576eab2.JPG)
![sales](https://user-images.githubusercontent.com/38730778/212720820-09add760-b979-49f8-8ed4-a322d966211e.JPG)
![purchase report](https://user-images.githubusercontent.com/38730778/212720823-34af56a2-1827-4d6f-abc1-7fd13cbaeac6.JPG)
![sales report](https://user-images.githubusercontent.com/38730778/212720825-0636c339-1897-4649-94d2-095625c09240.JPG)
