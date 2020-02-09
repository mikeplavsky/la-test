In Azure https://shell.azure.com/:
```
az ad app create --display-name la-test \ 
--oauth2-allow-implicit-flow true \
--reply-urls http://localhost:8000
``` 

Locally:
```
python -m SimpleHTTPServer
```

In browser go to: http://localhost:8000
Open Console and Run: 

```
await query_la("Console_01_23_4619234_CL | where TimeGenerated > ago(100d) | limit 10")
await query_la("Console_01_23_4619234_CL | where TimeGenerated > ago(100d) | where  Message contains 'error'")
```

Useful links: 

* https://azuread.github.io/microsoft-authentication-library-for-js/docs/msal/ 
* https://docs.microsoft.com/en-us/rest/api/loganalytics/query 
