# Bc26OpenCPU - MQTT    
Advise: Please read ***Quectel_BC26-OpenCPU_User_Guide_V10*** in /doc ;      
this project may not be perfect in function, just a demo; It can connect to MQTT server ,subscribe topic ,publish or recieve messages in 0/1/2 qos;          
## quick use     
>**make and download**      
>> OPEN BC26_OpenCPU_NB1_SDK_V1.3/MS-DOS      
>> use ***make clean*** to clean existing OBJ files;    
>> use ***make new*** to make APP file ,then use **Qflash tool** download APP file via serrial port; 
>> APP.C in ***./BC26_OpenCPU_NB1_SDK_V1.3/custom/***  contains the main_task . start from here;  
>>> note: make sure your module is BC26NBR01A07 or update this or newly factory file with **Qflash tool** first   

## MQTT Paras Set     
please refer to line 115 in APP.c replace the ~~~ mark with your own paras     
>MQTT_Para_t MQTT_para = {0, 0, 0, 0, 0, 0, NULL, NULL, NULL, NULL, NULL};      
>char SERVER_ADDR[] = "\" ~~~ \"\0" ;     
>char CLIENT_ADDR[] = "\" ~~~ \"\0" ;    
>char USERNAME_ADDR[] = "\" ~~~ \"\0" ;    
>char PASSWD_ADDR[] = "\" ~~~ \"\0" ;    
>char TOPIC_ADDR[] = "\" ~~~ \"\0" ;   
>char testpayload[] = "\" ~~~ \"";   

## updating...
