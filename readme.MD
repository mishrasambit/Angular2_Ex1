Angular 2 Fundamentals Course
========================
This is the getting started package for the Pluralsight course on Angular 2 Fundamentals found here: http://app.pluralsight.com/courses/angular-fundamentals

**Course Status**

The course is currently up-to-date.


Getting Started
---------------
Be sure you're running the recommended node version, which is 6.3.0+: `node --version`

Follow along with the course linked above. To start the server:

```
npm install
npm start
```

for facebook login
<fb:login-button autologoutlink="true" onlogin="OnRequestPermission();">
        </fb:login-button>

        <button onClick="callApi()">get email</button>
     <script src="http://connect.facebook.net/en_US/sdk.js"></script>
    <script language="javascript" type="text/javascript">
        FB.init({
            appId: '1665748113728904',
            status: true,
            cookie: true,
            xfbml: true,
            version: 'v2.4'
        });
        function callApi(){
            FB.api('/me', {fields: 'email'}, function(response) {
              console.log(response);
            });
        }
    </script>
