---
title: "API Clients - Chaining Requests"
date: "2017-03-20"
tags: 
  - "api"
---

POSTMAN

https://www.getpostman.com/docs/chaining\_requests

http://blog.getpostman.com/2014/01/27/extracting-data-from-responses-and-chaining-requests/

var jsonData \= JSON.parse(responseBody);

postman.setEnvironmentVariable("token", jsonData.token);

 

Add

{{token}}

* * *

PAW

## Variables from previous responses

https://paw.cloud/docs/environments/environments-from-responses

In the response view, right-click on the field you're interested in and pick _Copy as Response Body Dynamic Value_
