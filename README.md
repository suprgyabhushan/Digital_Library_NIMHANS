# Digital Library
1. Project work regarding Digital Library for NIMHANS!! We are using the DSpace open source repository to make our own IIITB or NIMHANS digital library.

2. This project is purely done in Linux environment. So Windows or MAC users bye!!

## How to install DSpace in Linux ?

1. Just have the softwares installed :-
  - Tomcat 7 Server
  - Java 7 JDK
  - Postgresql 9.3
  - Ant for building pages everytime we customize pages
  - Maven for installing packages in DSpace
  
2. Just follow the steps given in this <a href="http://dspaceclub.blogspot.in/2015/02/how-to-install-dspace-50-on-ubuntu-1410.html" target="_blank">Link</a>.

3. **Important Points to remember**
  - Before deploying pages on Tomcat 7 server, modifying the server.xml file of tomcat doesn't work. To solve this, just copy the webapps folder from /dspace/webapps to /var/lib/tomcat7/webapps
  
  ```sh
  sudo cp -R /dspace/webapps /var/lib/tomcat7/webapps
  ```
  - Do not forget to make a database name dspace in postgresql either in pgadmin (GUI form of postgresql just like phpmyadmin) with owner dspace login role with suitable authorizations. Without doing this, ant won't be able to build. 

## How to customize DSpace pages in Linux ?

1. There are two interfaces - XMLUI and JSPUI. To customize any of the pages, just go to the /dspace/webapps/*respective interface*.

2. Edit the JSP files in the /dspace/webapps/jspui to customize.

3. Edit the XML

4. Just see the corresponding reading material in the repo

## How to add more features in DSpace ?

## References

1. http://wiki.lib.sun.ac.za/index.php/SUNScholar/Install_DSpace
2. http://dspaceclub.blogspot.in/2015/02/how-to-install-dspace-50-on-ubuntu-1410.html
