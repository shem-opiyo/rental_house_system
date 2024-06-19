how to connect java projects in netbeans to mysql database in xampp
consider the video in the following link: https://youtu.be/olul_7oDzeg?list=PLtI-7v8oyD-H7Vp9jT93AmjKpstDv5ZmR

1. Search JDK (proceed to java downloads).
2. Download the java development kit (x64 installer) for windows/windows. Select the latest JDK version.
3. Download and install Netbeans. Then open Netbeans. 
4. Search and download Xampp, then start the Apache server and the mySQL server. click MySQL admin (button infront of mysql) to open the database management browser./ you can navigate to the welcome tab and click on go to application to open the database management browser.
5. in the browser browser window (phpmyadmin), click on user accounts.(The default username for MySQL is root without password. But you can create a new user.)
6. Under new, click on add user account/add new user. Then:
        - enter the username i.e. admin
        - enter the host name i.e. local
        -enter the pass word (optional)
        -grant all the necessary priviledges or click on check all (under the global priviledges box)
        - click on Go, then ok (new user successfully created)
        
7. Go to netbeans and click services tab. Right click database and create a new connection.under the drivers section (click on new drivers), then click on add. This will prompt you to select a mysql-java connector driver. (If you don't have it yet, you can dowload the connector. 
8. Go to the browser and search for mysql connector (click on the lick with connector/J). Select the platform independent option and download the zip file (then click on no thanks, just start my download).Extract the zip file to a specified folder. 
9. Then, go to Netbeans in the dialog box where you were to upload the connector, and add the downloaded jar file-'mysql-java-connector 8.0.3.3.jar', then click open, ok, and next.
10.  on the new connection wizard:
        * enter database name, enter the username, and password you created or if you didnt create a user account, you can use 'root' in the username and leave the password blank.(make sure the localhost is the same as the one used to create the user account).
        *then click on test connection. If the connection is successful, proceed to finish. (you have already connected the database to netbeans)
11. Rename the connection (under databases) by going to properties and change display name.
12. Go to the project you wish to work on or create a new project(with maven).
13. Go to the main class of the project, and create a connection class method. Enter the following details to create the class:
        - import SQL connection class
        import java.sql.Connection;
        - 

14. 
        

