# WELCOME!!!








# TASK-1:
download the index.html by
```
curl -o http://10.x.x.x/tezt/index.html

```
<img width="540" height="674" alt="image" src="https://github.com/user-attachments/assets/ee1e9767-9ba0-47bf-9266-7ba119ec8956" />

use , to containerize them
```
docker compose up -d

```

<img width="1394" height="155" alt="image" src="https://github.com/user-attachments/assets/733d1abf-0990-46f5-b1ef-d791abbdb1c0" />


check the active containers

<img width="569" height="163" alt="image" src="https://github.com/user-attachments/assets/283f8c85-2f61-44ef-b863-50a129bca9f5" />


this contains compose.yaml and the organizers index.html file

use curl to test them

<img width="460" height="43" alt="image" src="https://github.com/user-attachments/assets/3e7366b1-ddc4-4f7e-83e5-b252d87e660b" />

other wise go in browser and check the loading web page

<img width="967" height="400" alt="image" src="https://github.com/user-attachments/assets/23eeff96-7313-4a04-a93f-7d2e894d4f48" />








# TASK-2:

accessing the webpage using another device [mobile phone] 
```
CONCEPT: LAN: local area Network, by connecting the secondary  device to the same network that is used by the server,
we can view the changes in the web page
```
for that get the host system's ip address
```
ip addr or ip a

```
look for wlan0/lo

get the host's IP then use it in the secondary device as follows
```
http://10.10.152.71:8080 #use it u]in mobile

```

<img width="504" height="431" alt="image" src="https://github.com/user-attachments/assets/a3288510-4300-4138-b92f-dd84f1b6b362" />








# TASK-3:

now the changes made in the file should also reflect on the file

to login remotely i use ssh in host, then by logging i  would edit the index.html file

<img width="879" height="361" alt="image" src="https://github.com/user-attachments/assets/ffa4d798-06cf-4132-ac0a-ec7d2dbeb881" />


now in the same manner, lets refresh the tab in mobile which results in change of file

<img width="453" height="300" alt="image" src="https://github.com/user-attachments/assets/34bbc5b2-c91f-40dc-ae01-359374c10e34" />

```
This demonstrates the network functionality between server and the client

```



# TASK-4:

setting up another port [8081] on the same server, in which it hosts another webpage

let configure the compose file

<img width="707" height="503" alt="image" src="https://github.com/user-attachments/assets/2beb3aad-1042-44f0-9ca1-929628379bc2" />

then after compose

the result would be

<img width="458" height="269" alt="image" src="https://github.com/user-attachments/assets/c6dc4cc9-360c-4421-9c46-4268b6518c14" />

this webpage uses 8081 port number that is specified in the server .





# TASK-5:

Now we would make the http to https, other wise we would make 80[HTTP] to 443[HTTPS].
  
  * also configure the compose file 

for that we would need certificates [such as self-signed] 
see...
<img width="732" height="254" alt="image" src="https://github.com/user-attachments/assets/65357791-8ed1-4634-b146-cf033e3bc1db" />


these uses rsa cryptographic algorithm 


<img width="358" height="61" alt="image" src="https://github.com/user-attachments/assets/cf69c0c1-f406-4893-a7bb-824e75ccd3cf" />

now due to safety constraints the web page would show

<img width="953" height="711" alt="image" src="https://github.com/user-attachments/assets/ea4805e7-ab26-42fa-b7c9-e9b103d0ec10" />


then by proceed

<img width="650" height="308" alt="image" src="https://github.com/user-attachments/assets/eb2a9839-ae8e-46fe-b58e-52e23a7f41e1" />



also view the certificate on the webpage itself

<img width="785" height="752" alt="image" src="https://github.com/user-attachments/assets/d7aa3d77-ea55-420e-af94-de1742c15a7a" />





















# NOTE 
  in case of firewall blocking in the host system, configure the firewall itself

```
ufw or firewalld

```

<img width="743" height="98" alt="image" src="https://github.com/user-attachments/assets/f0568641-d6aa-4197-9fd0-8f3e1fd28de6" />



This would allow the inbound HTTP/HTTPS traffic for the specified ports 




# THANK YOU!!!


