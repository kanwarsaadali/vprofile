FROM mysql:latest

LABEL "Project"="vprofile"
LABEL "Author"="saad"

# Set the root password
ENV MYSQL_ROOT_PASSWORD="vprodbpass"

# Create a database and user
ENV MYSQL_DATABASE="accounts"

ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql