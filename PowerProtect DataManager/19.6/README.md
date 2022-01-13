# DELLEMC-DPS-Postman-Collections-RESTAPI for PowerProtect
Download or clone the repo and import PowerProtect 19.6 Environment.postman_environment.json and PowerProtect 19.6.postman_collection.json files into Postman.

## Power Protect Data Manager (PPDM) 19.6
Once you import collections and environment variables (both are JSON), you need to modify the following environment variables.

We are working with Postman Environment, so please also import the Postman Environment.  
To get this working in your environment you need baseUrl which can be in my example https://ppdm.vlab.local:8443  
username  <this is the PPDM username to login in / admin)  
password   < this is the password for the above user to login in PPDM>


After that config all calls are running and the needed accesstoken are added automatically!   

I have also some working UseCases
PPDM 19.6 - UseCase   
- PPDM 19.6 - Login  
    * Login and token creation  
- PPDM 19.6 UseCase - Add DD  
    * validation and cert acceptance to get a DD added into PPDM  
- PPDM 19.6 UseCase - Add vCenter  
    * validation and cert acceptance to get a vCenter added into PPDM
- PPDM 19.6 UseCase - Discover DataDomain  
    * start a discover job for a special DD
- PPDM 19.6 UseCase - Discover vCenter
    * start a discover job for a special DD
- PPDM 19.6 Use Case - create Policy  
    * create a PPDM policy PLC1 which we can use      
- PPDM 19.6 Use Case - Assign asset to a policy  
    * assign the asses "file" to the ppdm policy "PLC1"
- PPDM 19.6 Use Case - Trigger manual backup of a Policy
    * trigger one adhoc backup  
- PPDM 19.6 Use Case - VM Image Level Restore - to New VM  
    * restore single VM  

We started here with postman path variables which you should use and change for individual IDs int the gui
![](images/postnamepathvar.PNG)
The rest of the variables will be updated automatically based on the API response.

![](images/ppdm.PNG)
