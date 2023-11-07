# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
## Step 1:
Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
## Step 2:
Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/06beb414-2c6a-4c88-971a-bce07c2f1a9f)



## Step 3:
A new window will appear. Select “Simple Root Resource” and click Next.
 ![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/009b7bba-e93e-4472-bda7-e770cecbe8bf)

 


## Step 4: 
In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/07e603ca-2f6e-4f0e-8a47-42dd9bc0aaf6)


## Step 5:
Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
## Step 6:
Alter getHtml() method as shown below.
## Step 7:
Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/6afdb7fa-271b-4c07-bf81-4a45538c9d38)

 


## Step 8:
To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



### Client-Side:


## Step 1:
Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
## Step 2:
Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/050fa2d4-656e-44e9-a097-a0f18e1ecfbe)



## Step 3:
A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/683b4629-94d9-4e73-aed9-08b0091cb186)



## Step 5:
Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/08040408-4743-4d25-909d-14d2cc7cf60a)

## Step 6:
An editing tab will open. Alter getHtml() method with the following.
 
 ![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/de6e59b1-80e2-4e0c-a904-2c5817608c5b)



## Step 7: 
Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/407fa464-6bdb-4c25-af56-b2adc7ebf1a3)


## Step 8:
A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/076bd793-43ad-4c3d-a53f-4d5c68490f64)



## Step 9:
Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
## Step 10:
A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/490a96f8-6aed-473f-a008-76e090682fdf)

## Step 11:
Save the project and build it.
## Step 12:
Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/Vasanth1234567/Ex-04_RESTful_Web_Services/assets/86919099/66e0d7e1-b84c-4a9e-b111-081581cef0f9)



### Client-Side Remote Invocation:


## Step 1:
Follow steps 1-5 as in Section 2.2
## Step 2:
In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
## Step 3:
Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
