# DELLEMC-DPS-ReST-api DataDomain 7.3
This repository contains many ReST API collection for Postman https://www.getpostman.com/downloads/.
In this Postman collections I do work with an environment (postman_environment.json) where I define all variables needed to work with the ReST API like Server or login or auth token where needed and the api collection (postman_environment.json) where I do use this variables.
I also have added for the DELL DemoCenter Session a special environment you can import and use without any change.

Download the whole repository and play with all the collections and let me know what's working and what not.
If you download individual files make sure you really downloaded the json file and not a wrapped json file which will fail during import with a wrong format error.

Starting with DDOS 6.1. you also do have a DD ReST test client you can reach @ https:/{{DD-hostname}}/api/doc/ for playing around.    
Swagger file for general usage can be found @  
https://{{DD-hostname}}/api/doc/web_api.json

While there are some changes added to the repository like
{{baseurl}} which you need to change to https and the port as highlighted  
http://ddve-02.vlab.local:3009 i.E for a DD in my environment.   

Use Cases have been added to the latest Collection
* Use Case
    * Use Case - Create a new admin user
    DD System ID. Please change if not valid in your environment.
    * Use Case - Add a DDBOOST User - working with Path variable for the DD System ID. Please change if not valid in your environment.  
    * Use Case - Create a Storage Unit with user and limits  
    Create a storage unit and assign a DDBoost user. Make sure SMT is enabled- working with Path variable for the DD System ID. Please change if not not valid in your environment.

![1](https://github.com/juergenschubert/DELLEMC-DPS-ReST-api/blob/master/images/postman-env-var.png)

When logging into DD make sure you use the right environment and a login does create the auth token
![2](https://github.com/juergenschubert/DELLEMC-DPS-ReST-api/blob/master/images/postman-login-dd.png)

This auth token need to be used for all uri call for DD in this example  
![3](https://github.com/juergenschubert/DELLEMC-DPS-ReST-api/blob/master/images/postman-xauth-token.png)
