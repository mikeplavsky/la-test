In Azure https://shell.azure.com/:
```
az ad app create --display-name la-test --oauth2-allow-implicit-flow true --reply-urls http://localhost:8000
``` 

Locally:
```
python -m SimpleHTTPServer
```

Useful links: 

* https://azuread.github.io/microsoft-authentication-library-for-js/docs/msal/ 
* https://docs.microsoft.com/en-us/rest/api/loganalytics/query 
