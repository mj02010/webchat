# Chat
Web chat created for fun. Created in late 2020.

## Some Features
* To send an image, copy it to your clipboard and paste it while typing in the message form.
* Click on a name in the userlist to interact with user commands.
* Type "/cmds" to see a list of commands
* Mention a user (like "@user") to notify them about your presence.


## How to create admins
5	- If you decide to fork this, you can create an admin account by running the following these instructions.
6	-
7	- 1. Open the public/admins.json file. Make sure allowAdminCreation is set to true.
8	-
9	- 2. Run the following command in the chatroom's chat:
10	-   
11	-   /createadmin name color password
12	-
13	- 3. To join as an admin, enter your username as !yourpassword
14	-
15	-   So for example:
16	- I could execute /createadmin 7ih red ilikepie.
17	- Then, I would enter my username as !ilikepie.
18	-
### More about allowAdminCreation
20	- If this variable is set to true, anyone is allowed to create an admin account.
21	- If false, no one is allowed to create an admin account.
22	-
23	- I couldn't think of a more convenient way to let the site's owner create an admin account whenever.
24	-
25	- I would recommend setting it to false after you are done creating an admin account to prevent anyone else from creating their own admin account.
26	-
### How to delete admin accounts
28	- If you want to delete an admin account, open the admins.json file and just delete the admin objects with the admin names that you want to remove.
29	-
30	- For example:
31	- If I wanted to remove the Zero account, my code would change from this:
 ```
 {
 "allowAdminCreation": false,
  "admins": [
   {
    "name": "Statix",
    "color": "#cc5500",
    "password": -1502145674
   },
   {
    "name": "Zero",
    "color": "#009e60",
    "password": -1136902589
   }
  ]
 }
 ```
...To this:
 ```
 {
  "allowAdminCreation": false,
  "admins": [
   {
    "name": "Statix",
    "color": "#cc5500",
    "password": -1502145674
   }
  ]
 }
```
62	-
63	- Keep in mind JSON has strict syntax, I would recommend pasting the file into [a json validator](https://jsonformatter.org/) to make sure there are no errors.
64	- The most important thing to remember is that JSON doesn't allow [trailing commas](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Trailing_commas).