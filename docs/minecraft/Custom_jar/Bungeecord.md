---
layout: default
title:  "Bungeecord"
parent: Custom-jar
grand_parent: Minecraft
permalink: /Minecraft/Custom-jar/
tags: Falix Bungeecord bungee cord custom jar custom-jar
---

# How to setup Bungeecord using a custom jar

## Part 1: Make at least 3 servers
+ A server with at least 512 MB ram, name this “Bungee”.
+ A server with at least 2 GB ram, name this “lobby”.
+ A server with at least 2 GB ram, name this anything you want.
+ Make more servers if needed, name it anything you want.

### The server named lobby will be the Lobby/Hub, the one named “Bungeecord” is where we will set up the bungee cord, and the other servers are destination servers.

![image](https://i.imgur.com/HRp80t4.jpg)
###### you can add as many servers as you want to the destination servers
###### server 1 and server 2 are both destination servers.



## Part 2: setting up bungee cord.
1. Go to the [bungee cord download page](https://ci.md-5.net/job/BungeeCord/).
2. Click on the bungee.jar file, it should download it.

![image](https://i.imgur.com/dnaIBd2.png)

3. Rename the file to “custom.jar”.

![image](https://i.imgur.com/a0svDyc.png)

4. Go to the [Game panel](https://panel.falixnodes.net).
5. Select your bungee cord server.

![images](https://i.imgur.com/dv8Cp4v.png)

6. Go to the file manager.
7. Upload the file we downloaded before.

![image](https://i.imgur.com/dCt2LzK.png)

8. Follow the guide [here](https://docs.google.com/document/d/1iod3fFZ1NvKfDuQxNsyVD3ea-uFJmaTaelVxAe9Io0U/edit?usp=sharing) to set the java version.
9. Go to the console, then start the server.
10. Wait until it looks like below.

![image](https://i.imgur.com/mI9oFVk.png)

11. Stop then kill the server. 
###### (the status panel always says starting for bungee, ignore it, you must also always kill your bungee server to turn it off)
12. Go back to the file manager.
13. Open “config.yml”.

![image](https://i.imgur.com/JuBOqSE.png)

14. Scroll down and find this, this is what we are interested in 

![image](https://i.imgur.com/WXWS9bj.png)

15. Remove the entire thing and paste the code below instead of it. Then make changes according to what it says in the code.

```YAML
servers:
  server 1:
    motd: '&1Just another BungeeCord - Forced Host'
    address: SERVER_1_IP:PORT
    restricted: false
  server 2:
    motd: '&1Just another BungeeCord - Forced Host'
    address: SERVER_2_IP:PORT
    restricted: false
  lobby:
    motd: '&1Just another BungeeCord - Forced Host'
    address: HUB_IP:PORT
    restricted: false
```

+ Server 1= change it to the name to your first destination server,
address:  change to IP:PORT of the first server
+ Server 2= change it to the name to your second destination server,
address:  change to IP:PORT of the second server
+ lobby  = keep the same,
address:  change to IP:PORT of the Hub/Lobby

### This is what mine looks like

![image](https://i.imgur.com/99ZRXGT.png)

###### I am only using 1 destination server

### Add all your servers except the bungee server. (remove server 2 if you are using only 1 destination server and add more if you are using more)

16. Scroll down until you see `host: 0.0.0.0:25577`
17. Change `25577` to your bungee cords server port, then save the file

![image](https://i.imgur.com/qZM4FgS.png)

18. Save the file and start the server.

## Step 3: How to set up the lobby and destination servers.

19. Setup all the servers (other than the bungee server).
20. Go to the file manager
21. Open server.properties then find online-mode and set it to false

![image](https://i.imgur.com/Mn4LRcd.png)

22. Then save the file and go back to the file manager
23. Open spigot.yml, find bungee cord and set it to true

![image](https://i.imgur.com/KmTVABi.png)

24. Save the file then start the server

### Do that for all the servers other than the bungee cord server

## Last steps:

### Restart all your servers, then use the bungee cord server IP and port to join the hub/lobby.

### Once you join the hub/lobby use the command `/server <server_name>` to join your destination servers.
