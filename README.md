# travel-buddy-app-oauth-implicit-grant-flow

Edited pom.xml to run tomcat in https mode. Now Facebook supports only HTTPS Callback URLs.

Execute following command in the project folder to generate self signed key. (https://www.logicbig.com/tutorials/misc/java-ee-server/apache-tomcat-https.html).

<code> keytool -genkey -noprompt -alias tomcat-localhost -keyalg RSA -keystore localhost-rsa.jks -keypass 123456 -storepass 123456 -dname "CN=tomcat-cert, OU=Dev, O=Logicbig, L=Dallas, ST=TX, C=US" </code>

Run using command

<code> mvn tomcat7:run-war </code>
