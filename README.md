Distributed Systems Sample Code
===============================

This is an improved version of the Distributed Systems sample code. This
actually deploys to Personal Tomcat correctly and reads credentials from
s3credentials.properties. Pull requests are welcome for improvements but
obviously not for implemented solutions.

Deployment
----------
On a lab machine/shell, run mktomcat7 <tomcatdir>. This produces a personal
Tomcat directory called <tomcatdir> and you can change the port by editing conf/server.xml and 
changing the value in the Connector tag lower down, NOT in the Server tag.

When you want to deploy a new version:

1. Using your IDE export to WAR file (using Eclipse, File -> Export -> Web -> WAR).
2. Place this WAR file in <tomcatdir>/webapps.
3. In <tomcatdir> run tomcat7 run.
