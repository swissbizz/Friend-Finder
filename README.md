# Friend-Finder

## Directions

To run Friend Finder, you will need Bash, Node, npm, and Heroku.

In Bash, type git clone git@github.com:https://github.com/swissbizz/Friend-Finder to download Friend Finder.

To use your own database, you will also need MySQL Workbench.

On Heroku, you can use either ClearDB or JawsDB. Both provide a free-tier option.
For JawsDB, type heroku addons:create jawsdb, then heroku config:get JAWSDB_URL to find (in the order of appearance) your username, password, hostname, port number, and default schema.

Open the file app/data/friends.js, change the values on lines 13 - 17, and type git push heroku master in Bash to apply the changes.

To seed your database, open MySQL Workbench and click Setup New Connection.

Enter your username, hostname, port number, and default schema. Once you click on OK, you will be asked for the password.

Finally, connect to your database and run app/data/friend_finder_db.sql.

And that should work!
