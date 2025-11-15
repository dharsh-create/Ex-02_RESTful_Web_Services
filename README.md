# Ex-02_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

<img width="864" height="277" alt="image" src="https://github.com/user-attachments/assets/2e25ac14-e3b2-4e09-8a65-40aee4014c65" />




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 <img width="718" height="503" alt="image" src="https://github.com/user-attachments/assets/8a006152-c2ab-414e-b082-004980ba4d65" />

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

<img width="774" height="536" alt="image" src="https://github.com/user-attachments/assets/0d682501-3632-48ad-ab38-45a2871f5a9a" />



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.

<img width="842" height="275" alt="image" src="https://github.com/user-attachments/assets/6925881a-7f10-4310-8f6d-5c9191e53e45" />

 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

<img width="859" height="599" alt="image" src="https://github.com/user-attachments/assets/437b5e95-a4c7-4625-8441-f3925548848e" />





Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.


Step 6: An editing tab will open. Alter getHtml() method with the following.

 <img width="857" height="480" alt="image" src="https://github.com/user-attachments/assets/5e255627-9a80-40a8-8bab-bcd0ba91be31" />

 <img width="811" height="279" alt="image" src="https://github.com/user-attachments/assets/eda8bc32-632b-430b-9f75-deba532f4282" />


 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

<img width="458" height="436" alt="image" src="https://github.com/user-attachments/assets/094ce62a-aa9e-4014-8bcc-7e602dffbada" />

 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

<img width="866" height="477" alt="image" src="https://github.com/user-attachments/assets/50e295a9-56ae-4cbf-930b-e01c0cad7d89" />



Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2

<img width="751" height="271" alt="image" src="https://github.com/user-attachments/assets/7ec3d210-d920-41bf-b88f-bf274f90575d" />


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
