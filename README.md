# project3 encryption example
Example of storing encrypted password in database and verifying against encrypted password


### To run this example: 
1. clone this repository using `git clone https://github.com/UCI-Chenli-teaching/2019w-project3-encryption-example.git`
2. open Eclipse -> File -> import -> under "Maven" -> "Existing Maven Projects" -> Click "Next".
3. For "Root Directory", click "Browse" and select this repository's folder. Click "Finish".
4. Go to `UpdateSecurePassword.java`, make sure to change your mysql username and password. 
5. Run `UpdateSecurePassword.java` on your local machine, it will update the passwords in your existing moviedb customers table from plain text to encrypted string.
6. Go to `VerifyPassword.java`, also change your mysql username and password. This program will verify if the email and password are valid.


To run it on AWS under command line:
1. clone this repository using `git clone https://github.com/UCI-Chenli-teaching/2019w-project3-encryption-example.git`
2. `cd 2019w-project3-encryption-example`
3. change your mysql username and password in `UpdateSecurePassword.java` and `VerifyPassword.java`
4. `mvn compile`
5. to run `UpdateSecurePassword`: `mvn exec:java -Dexec.mainClass="UpdateSecurePassword"`
6. to run `VerifyPassword`: `mvn exec:java -Dexec.mainClass="VerifyPassword"`
7. When execute java program using maven in command line, if the program doesn't exist after it finishes, you can just kill it.
