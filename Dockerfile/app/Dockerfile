FROM tomcat:8-jre11

LABEL "Project"="vprofile"
LABEL "Author"="saad"

# Remove the default Tomcat webapps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy your webapp to the container
COPY target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war

# Expose the Tomcat port
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]

WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps
