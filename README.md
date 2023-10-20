# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

<img width="317" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/ab77d3f2-e099-43c8-9c0e-50ac43e59b01">



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 

<img width="282" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/ca86dcce-fb6f-48b2-82ea-7fd8a6f78694">



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.


<img width="303" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/077df2ec-f327-4ed8-ba4f-6a3e2bee96ef">


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 <img width="319" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/848f46dc-e23a-4014-b62c-1ae8bbe492e8">



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


<img width="324" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/3f896dd4-5509-44f1-9f84-0d195eb5df65">


Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 

<img width="318" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/ce8cb4fd-8edc-42a8-ace8-d356cd77bc44">


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.


<img width="317" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/bc1460fc-51d7-4cf9-8325-58985a4e6fcc">


Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 

<img width="294" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/ab0d49c9-ab3a-4203-b82c-7fbe255d16d7">


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


<img width="180" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/aeb5ae2a-959b-4489-9829-af2e23d3835d">


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 
<img width="329" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/578c3af4-5668-4598-a898-9e70c536cd19">


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.



<img width="329" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/0f0987fa-4697-453d-8a71-ad90a2c031fd">

Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
<img width="388" alt="image" src="https://github.com/Srujana0303/Ex-04_RESTful_Web_Services/assets/132996836/3956f758-7fcc-4ee9-8004-0956f9f72667">


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
