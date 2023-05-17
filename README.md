# Hesk Ticketing
Hesk ticketool to docker container

# Prerequisite

Docker, docker-compose.

# Building and running with docker-compose

add chmod +x /hesk/script/entrypoint.sh

type this command : docker-compose build && docker-compose up &

This might take a few minutes so be patient! Once the container is up, move on to the next step.

# Website

Once the container is up and healthy, navigate to http://localhost:8000/install/

In the top left of the screen, you should see our custom header. Click Install and perform the following.

# DB info

- Database host : localhost
- Database name : hesk
- Database user : root
- User password : empty

# Delete install folder

On the following page you will see more instructions. If you click Skip Directly to Settings.

To clean the install folder go to http://localhost:8000/dash.php 

Click Remove "install Dir" and then "Admin"

# Dump/Restore DB

Go at http://localhost:8000/dash.php

 
Now click Dump Database

 
On your local, navigate over to the data directory and you should now see two files.
 

    dump.sql
    hesk_settings.inc.php

 
The dump file contains all of the data and setup you just did, and the php file contains the setup configurations 

 
# Credits

Thanks to scottyfullstack for the dash.php/entrypoint.sh

