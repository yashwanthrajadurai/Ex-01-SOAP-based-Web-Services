# Ex-01-SOAP-based-Web-Services

## Aim:

To create and execute SOAP-based web service program using server, client and client- side remote invocation.

## Procedure:

### Server-side:
#### Step 1:
Open NetBeans IDE.
#### Step 2:
Click File->New Project. Choose Java Web and then Web Application and click Next.
![2](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/53b21d93-3784-4a69-b64a-ac255b66a132)




#### Step 3:
Give your Project a suitable Name and then click Next.
#### Step 4:
In the next window, make sure you have selected Server as “GlassFish Server” and Java EE Version as “Java EE 7 Web”. Click Finish.
 ![4](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/ba86ef64-1e67-4eba-9935-96d4b158fcde)

 


#### Step 5:
Your new project will appear in the Projects tab in the left-most part of NetBeans.

#### Step 6:
Right click your Project and select New->Web-Service.

![6](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/e45c5bec-b36c-4b91-87c3-f49ac1c84604)



#### Step 7:
In the new window, give your web service a name and a package name. Click Finish.
 
 ![7](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/f6e330f4-a62a-44bb-9ce1-53e54db577f4)



#### Step 8:
A new coding tab will open that contains your web service.

#### Step 9:
Expand the folder “Web Services” under your project. You should see your newly created web service. Right-click on it and choose “Add Operation”.

![9](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/c0dc772c-c5ff-466f-bc8a-908a1f956291)




#### Step 10:
A new window to add operation will appear. In that give Name, Return Type to your operation. Then click the Add button to add necessary arguments/parameters for that
 
operation. (Since we are demonstrating simple addition, we use two arguments/parameters.) Once you are happy with your parameters/arguments, click OK.

![10](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/2e04e804-2aad-4074-87cf-2a9ed8b0fd78)


#### Step 11:
NetBeans will automatically generate the skeleton for the operation which will be like,

![11](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/eaf6cf88-92e2-478f-a6ac-f800251e6bd5)



#### Step 12:
. Replace return 0.0 with return (a+b)

#### Step 13:
Save your project. Right-click on the project, select “Clean and Build”. Once the Building process is successful, again Right-click on the project, select “Deploy”.
Deploying might take time depending on the size of the project. 

### Step 14:
Once your project is successfully deployed, right-click on your web service name and select “Test Web Service”
 ![14](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/4c82ecec-fe36-4826-96bb-37dd25bb0f75)

 


#### Step 15:
A new browser window will appear which will look like this

![15](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/1f23a946-d82a-440d-9435-14ea8a0d4907)



#### Step 16: 
You can give inputs to your web service and check whether it is working properly or not. If it is working properly, you will get a page like this
 ![16](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/4a6cac39-12aa-42c7-8495-77e777e89bcb)

 
### Client-side:


#### Step 1:
Create a new Java Web Project in NetBeans. (Follow Steps 1-5 as in section 1.1)
#### Step 2:
Right-click on the project and select New->Web Service Client.

![c2](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/3e65b81f-b2c5-4dac-af34-5b3850020e56)



#### Step 3: 
A new window will appear. Select “Project” under the heading “Specify the WSDL file of the Web Service.” and click Browse

#### Step 4: 
A new window will appear, in that carefully choose appropriate web service and click OK.
 ![c4](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/b4050bbd-3c0c-4c57-b6cb-27325f140340)

 
#### Step 5:
The Project file will be filled with the location to the WSDL file of the web service. If you prefer, you can give a package name. Or else click Finish
 ![c5](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/8bb6e72e-8085-42c6-b88e-db310a49605a)



#### Step 6:
In the Output Window at the bottom of NetBeans, you can notice that the client gathers the operations available in the web service.

#### Step 7:
Once it is done, you should see “BUILD SUCCESSFUL”.

#### Step 8:
Right-click on “Web Pages” under your Project and select “JSP”.

![c8](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/4053beb0-00c4-4f5a-8a7b-7f961b885084)

#### Step 9: 
A new window will appear, give a name to your jsp page and click Finish.

#### Step 10: 
Expand the folder named “Web Service References”-> “Addition” “Addition” “AdditionPort”. Once expanded you should see all the operations available in your web service.

#### Step 11: 
Carefully drag “add” operation and drop it into the JSP page. NetBeans will automatically create the code for invoking this operation which will be like,
 
 ![c11](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/b37ebd64-c3c4-4e9c-9ba4-bf41c6b246bb)



#### Step 12: 
Give values to your arguments and run the JSP file. 

#### Step 13:
A new browser window with the output will appear. 

### Client-Side Remote Invocation

#### Step 1: 
Follow Step 1 and Step 2 as in Client-side (section 1.2).

#### Step 2:
A new window will appear. Select “WSDL URL” under the heading “Specify the WSDL file of the Web Service.” and type the URL of the web service’s WSDL file. (Typically, the URL of the form http://ip:8080/Proj_name/Webservice_name?wsdl)
 

![cr2](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/7d6eb944-5735-40b1-a5fc-7af19d6b92c8)

#### Step 3: 
The remaining procedure is the same as the Client-side.


## Result:
Thus, the SOAP based addition program using Web service is executed successfully.
