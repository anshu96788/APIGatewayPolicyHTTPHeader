#  Webmethods.io API Gateway Securing APIs using HTTP Headers
## Getting Started
  This article explains about how to secure API’s using HTTP Headers.
 ## Prerequisites
 An account in [Webmethod.io API Gateway](https://www.softwareag.cloud/site/product/webmethods-api.html).
## Configuration
### Create a application
1. Login to your API Gateway tanent. And click on `Applications` tab from the menu bar. </br>
![image](https://user-images.githubusercontent.com/60179170/90880775-aafda200-e3c6-11ea-8ce6-562b1a8f8e13.png)
2. Create a new application by clicking `Create application` Button.
![image](https://user-images.githubusercontent.com/60179170/90880913-de403100-e3c6-11ea-834c-63c17b970065.png)
3. Give the application a name and click on `Continue To Indentifiers` Option.
![image](https://user-images.githubusercontent.com/60179170/90881038-134c8380-e3c7-11ea-91b9-853061462358.png)
4. Go to the Header key value text box and fill up the value you want to use as a identifier. Click on `Add`.
![image](https://user-images.githubusercontent.com/60179170/90881151-4727a900-e3c7-11ea-829f-0cf21b0ed565.png)
5. Click on the `Save` button present on top right corner.</br>
![image](https://user-images.githubusercontent.com/60179170/90881450-d634c100-e3c7-11ea-8a9c-cb2db0af646a.png)
### Add the application to the API
1. Now Click on `API` tab from the menu bar. </br>
![image](https://user-images.githubusercontent.com/60179170/90881674-417e9300-e3c8-11ea-8e73-33b336189342.png)
2. From here select the API which you want to configure. <b> If you dont have a API please [Visit this URL](https://github.com/SoftwareAG/webmethods-api-gateway)</b>.
![image](https://user-images.githubusercontent.com/60179170/90881768-71c63180-e3c8-11ea-8484-c5631c4e9dbc.png)
3. Now click on `Edit` Button and click `Yes`. </br>
![image](https://user-images.githubusercontent.com/60179170/90882023-da151300-e3c8-11ea-854d-5bf9d34c7244.png)
4. Now Click on `Application` Tab.</br>
![image](https://user-images.githubusercontent.com/60179170/90882109-09c41b00-e3c9-11ea-97ef-06871d2987ad.png)
5. Now in the search bar type the application name that you have just created and click ok.
![image](https://user-images.githubusercontent.com/60179170/90882177-2bbd9d80-e3c9-11ea-92b7-02b45cec2705.png)
### Add scope to the API 
1. Click on the `Scope` from the menu bar and select `Add scope`.
![image](https://user-images.githubusercontent.com/60179170/90882652-e9489080-e3c9-11ea-8db1-97f89f509131.png)
2. Give the scope a name and add the resources where you want to add the scope.
![image](https://user-images.githubusercontent.com/60179170/90882793-2f9def80-e3ca-11ea-942a-8e86f6605b26.png)
### Adding Policy
1. Click on `Policies` tab and select your scope.</br>
![image](https://user-images.githubusercontent.com/60179170/90882892-5e1bca80-e3ca-11ea-900e-0e7072843a4d.png)
2. Now from the `Policy Catalog` select `Identify & Access` and add `Identify & Authorize Applicaton` and check `HTTPHeaders` and keep the drop down option as `Registered applications`.
![image](https://user-images.githubusercontent.com/60179170/90883049-b18e1880-e3ca-11ea-8bbd-914a09fac37d.png)
3. Now click on `Save`.
### Test using Postman
1. Coppy your gateway end point and paste in Postman.
![image](https://user-images.githubusercontent.com/60179170/90883606-ca4afe00-e3cb-11ea-8ec7-73605653e990.png)
2. Add all the HTTP header you configure in your API.
![image](https://user-images.githubusercontent.com/60179170/90883755-1007c680-e3cc-11ea-953f-5f0f415e759e.png)
3. <b>Now add the extra header which you have configure in the application. As you have configure securing APIs using HTTP Headers.</b>
![image](https://user-images.githubusercontent.com/60179170/90884536-9244ba80-e3cd-11ea-80f7-d5fd34041812.png)
4. Now send the request and you will get 200 OK response.
![image](https://user-images.githubusercontent.com/60179170/90884674-cddf8480-e3cd-11ea-9f04-b260f961d267.png)
5. If you remove the extra header then you will get error.</br>
![image](https://user-images.githubusercontent.com/60179170/90884838-1dbe4b80-e3ce-11ea-9cc1-4e7d10cec21e.png)

