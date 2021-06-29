---
layout: default
title:  "Getting Started"
nav_order: 1
parent: General
grand_parent: Minecraft
permalink: /minecraft/general/getting-started/
tags: minecraft message motd color create creating configure configuring ip address connecting server icon installing eula optimize lag tps egg multiegg properties load purpur
---

<video controls poster="https://i.imgur.com/ofhQdwK.png" src="https://files.catbox.moe/7q42gz.mp4"></video>

# Creating a Server
## Creating a Server on your Account
To create a Minecraft Java server, go to your Client Panel. On the left sidebar, choose Create Server. Type in all required information like server name, memory amount, and server location. Once done, click the Create button and wait at least a minute in the Client Panel for the new server to be created for your account.

Now, in the [Game Panel](https://panel.falixnodes.net/) you should see the new server on your server list. If the server list indicates that it is still installing, wait at least 2 to 5 minutes for the installation to be complete. If the installation is taking longer than usual (over 5 to 10 minutes or more), head back to your [Client Panel](https://client.falixnodes.net/) and delete, then re-create the server.

## Starting the Server
 Select your new server and go to the Console tab, usually already selected by default. Click the Start button, located in the upper left corner of the Console tab. You're going to be selecting which type of server you want during the first startup of your new server. In this case, we're creating a Minecraft Java server, to select Minecraft Java, then the type of Minecraft Java server that you want like Vanilla or PaperMC, and select the version of Minecraft Java you want to play on.
 
Click "I Accept" when the **Mojang EULA** pop up appears. The server is turn off for a few moments, then turn back on, and will continue to boot.

During the first boot of any Minecraft server, it may take a while to prepare spawn area.

## Using a Custom Jar
Minecraft uses a __.jar__ file to start your server and setting a custom jar is easy.
If the option you want isn't available on the first boot, a custom jar can be used. Simply upload the .jar file(e.g. __paper-1.16.5-774.jar__) to your server's root directory in files, then rename it to __custom.jar__. You can rename the file by clicking or tapping on the three dots on the right side, then clicking Rename.

Falix will automatically detect the __custom.jar__ on the next launch of your server and will use the file to boot.

# Choosing Your Server Java Version
<!-- # What is Java? (An explantion for noobs will be added later on) -->
## Minecraft Versions
Use **Java 8** for Minecraft 1.12.2 or older

Use **Java 11** for Minecraft 1.13 or newer

Use **Java 16** for Minecraft 1.17 or newer

## Set a Default Version
> Make sure your server is turned off before doing the next steps.

To make a Java version the default one, so that you don't need to select it every time you start your server, visit the [game panel](https://panel.falixnodes.net/), find and click on your server, find the "Startup" page on the top bar, scroll down to "Variables", then find "JAVA VERSION" and type the following for:

## Java8
`adopt@1.8.0-292`

## Java11
`adopt@1.11.0-11`

## Java 16
`adopt@1.16.0-1`

## Other java versions:

| Java version      | java code          |
|:---------------|:----------------------|
| 8              | adopt@1.8.0-262       |
|                | adopt@1.8.0-265       |
|                | adopt@1.8.0-272       |
|                | adopt@1.8.0-275       |
|                | adopt@1.8.0-282       |
|                | adopt@1.8.0-292       |
|:---------------|:----------------------|
| 9              | adopt@1.9.0-0         |
|                | adopt@1.9.0-4         |
|:---------------|:----------------------|
|10 | adopt@1.10.0-2|
|:---------------|:----------------------|
|11 | adopt@1.11.0-8|
|| adopt@1.11.0-9|
|| adopt@1.11.0-10|
|| adopt@1.11.0-11|
|:---------------|:----------------------|
|12 | adopt@1.12.0-0|
|| adopt@1.12.0-1|
|| adopt@1.12.0-2|
|:---------------|:----------------------|
|13 | adopt@1.13.0-0|
|| adopt@1.13.0-1|
|| adopt@1.13.0-2|
|:---------------|:----------------------|
|14 | adopt@1.14.0-0|
|| adopt@1.14.0-1|
|| adopt@1.14.0-2|
|:---------------|:----------------------|
|15 | adopt@1.15.0-0|
|| adopt@1.15.0-1|
|| adopt@1.15.0-2|
|:---------------|:----------------------|
|16 | adopt@1.16.0-0|
|| adopt@1.16.0-1|
|:---------------|:----------------------|

Now, go back to your console, start your server and you'll see it using the Java version you set.

> If the above does not work, manually delete the `.jabba` folder and restart your server.

# Accepting Mojang's EULA
If for whatever reason clicking "I Accept" didn't work when creating your server, you can still accept the EULA manually.

In order to start your server, you must accept [Mojang's EULA](https://account.mojang.com/documents/minecraft_eula). If you agree to it, go to your server's file manager, find and open the file "`eula.txt`", find the "`eula`" string and set it to `true`.

# Optimizing your Server
Optimizing your server is a great idea to reduce lag and server load, as it increases the efficiency of the server, letting it process requests quickly. By doing this, you will also increase TPS.

## Pre-requisites
Choosing the right server type is very important. An example of a good server software type is [Purpur](https://purpur.pl3x.net/), as it is very optimized and provides a ton of configuration options.

## How do I optimize my Server?
You can find a detailed guide [here](https://www.spigotmc.org/threads/guide-server-optimization%E2%9A%A1.283181/) for PaperMC, or you can use [this one](https://github.com/YouHaveTrouble/minecraft-optimization) for Purpur or other PaperMC forks.
These guides give a detailed explanation of all the settings they do on your server. To use them, go to the said files and configure them as the guide shows.

You also have a shortcut. You can check out premade configs by clicking [here](https://github.com/flaxeneel2/pterodactyl-optimized-paper-egg) and then edit the values to your liking (PaperMC).

# Configuring
## Message of the Day
Also known as MOTD, is the message that shows up below the server name on a multiplayer server list. Usually used to say what's new about the server and/or also displaying what version it supports. Sometimes also used to indicate what games it has to offer or just a short description of the server.

To configure MOTD(Message of the Day), the setting for this is usually found in the server.properties file. Simply just change it to what you want for your Minecraft Java Server.

If you're interested in changing text colors, use these color codes:

| Preview        | Color Code                                      |
|:---------------|:---------------------|:-------------------------|
| <span id="black_color" class="color-block"></span> Black | \u00A70 |
| <span id="dark_blue_color" class="color-block"></span> Dark Blue | \u00A71 |
| <span id="blue_color" class="color-block"></span> Blue | \u00A79 |
| <span id="dark_green_color" class="color-block"></span> Dark Green | \u00A72 |
| <span id="green_color" class="color-block"></span> Green | \u00A7a |
| <span id="dark_aqua_color" class="color-block"></span> Dark Aqua | \u00A73 |
| <span id="aqua_color" class="color-block"></span> Aqua | \u00A7b |
| <span id="dark_red_color" class="color-block"></span> Dark Red | \u00A70 |
| <span id="red_color" class="color-block"></span> Red | \u00A7c |
| <span id="dark_gray_color" class="color-block"></span> Dark Gray | \u00A78 |
| <span id="gray_color" class="color-block"></span> Gray | \u00A77 |
| <span id="dark_purple_color" class="color-block"></span> Dark Purple | \u00A75 |
| <span id="light_purple_color" class="color-block"></span> Light Purple | \u00A7d |
| <span id="gold_color" class="color-block"></span> Gold | \u00A76 |
| <span id="yellow_color" class="color-block"></span> Yellow | \u00A7e |
| <span id="white_color" class="color-block"></span> White | \u00A7f |

## Server Icon
The server icon helps indicate the branding of your Minecraft Java server, it's easy to set one. Simply create an icon that is 64x64 in resolution. Name the server icon as <u>server-icon.png</u> and add it to the root of your Minecraft Java server files.

## Player Limit

By default, Minecraft sets 20 as the max player limit for Minecraft Java servers. You can increase this, or decrease, to any number you want. To configure the player limit, the setting for this is usually found in the server.properties file. Simply, just change the number 20 to something else, you could also set -1 for unlimited.

# Setting Operators

<video controls poster="https://i.imgur.com/G5OiZdi.png" src="https://files.catbox.moe/i9tgsz.mp4"></video>

An operator is a player with administrative access to your server, giving them full access to all commands. Even commands like /stop or /restart.
To set an operator, use:

```
/op Username
```

As an example, if you wanted to op Notch, you would use:

```
/op Notch
```

If you ever need to remove a player as operator, you could replace `/op` with `/deop`

Please don't use `/` in the Console tab, or will output as "unknown command". `/` should only be used in-game.

If you want to give some players access to specific admin commands, but not everything, you can use [LuckPerms](https://luckperms.net/) for this, which we all recommend.

# Connecting
## Find your Server IP Address
In your [Game Panel](https://panel.falix.gg/) the IP is shown in the upper left on the Console tab. Use this to connect to your server. It should look something like __de##.falixnodes.net:#####__.

If you're looking for the numeric IP, this usually shows up when booting the server.

## Play In-Game
On your Multiplayer server list, click Add Server, then put the IP for your server into the IP Address box. As for the Server Name, this can be set as whatever. Click Add and the server should appear on your list.
