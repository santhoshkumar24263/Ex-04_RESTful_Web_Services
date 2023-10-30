# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.



![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/8e74a34f-724e-4583-b60a-19177c93d82e)





Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 

![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/c9d7499a-4d7a-42b7-b0db-52d3e1cdd08b)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.


![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/e798869c-7e88-4ba4-8441-395984be2c3c)




Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

[Uploading image.png…]()

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/4b616116-2e2a-4547-9941-6a91f842e899)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 
Step 4: Carefully select your RESTful resource (web service) and click OK.


![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/c6cc1677-acbf-4529-a2cd-593672844baa)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.


![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/1344f71e-9475-4b63-ad65-800c0a0ff0ff)



Step 6: An editing tab will open. Alter getHtml() method with the following.
 

![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/9dc874ce-a941-4a6c-8e18-1fbb4c69bc84)



Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/630d241c-4d05-4a44-b7a1-6b0ef1b8aff5)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 

![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/1b2f767a-f135-41e5-8167-d5df7f4e5190)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/a13ea146-7cfe-4064-ab7e-aec3c9964404)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/santhoshkumar24263/Ex-04_RESTful_Web_Services/assets/127171952/352c3a28-1282-4947-aa87-9720877522cd)



Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
