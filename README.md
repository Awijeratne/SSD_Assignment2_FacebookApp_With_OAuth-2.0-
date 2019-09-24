1. Create a Facebook app in developers.facebook.com

   You have to create an application in the developer account on Facebook. You can go to https://developers.facebook.com/ and add a
   new application.
   
   Give a display name and contact email in order to create the application.
   
   In the Settings section of the "Facebook Login", there is a place to provide the Redirection Endpoint URL which must be included 
   in client web application and Facebook sends responses to this URL.
   
   Go to the Dashboard -> Settings -> Basic, you can find the App ID and the App Secret for the app. In OAuth terminology, it will 
   call the same Client ID and Client Secret which is display here.
   
2. Bootstrap Spring Boot application

   Go to the Spring Initializr page and download the initial application.
   
   Check whether all the dependencies available in the pom.xml file.

3. YAML properties configuration

   Create an application.yml file and add the oauth2 setting with App ID and the App Secret.

4. Web security configuration

   Add EnableOAuth2Sso annotation to the main class.
  
   Modify the main class with WebsecurityConfigurerAdapter and override the configured method.

5. Rest controller

   Add RestController annotation to the main class and implement the method.

6. Static web page to connect Facebook

   Create an index.html file inside the static folder with basic HTML designs.
