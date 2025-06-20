# Use official Tomcat base image
FROM tomcat:9.0

# Set environment variable to reduce download size
ENV CATALINA_HOME /usr/local/tomcat

# Download sample.war and deploy to webapps
RUN apt-get update && apt-get install -y wget && \
    wget https://tomcat.apache.org/tomcat-7.0-doc/appdev/sample/sample.war -O $CATALINA_HOME/webapps/sample.war && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Expose port
EXPOSE 8181

# Start Tomcat (inherited from base image)
CMD ["catalina.sh", "run"]

