# HP-OO learn-chef Content Pack

## Introduction

This HP-OO learn-chef Content Pack is intended to demonstrate the integration between HP-OO and Chef 12.6.
While these flows have been tested on learn-chef environment, they also shall work with other Chef 12.6 environments.

These flows are based on [HP-OO Chef Content Pack 1.1.4] (https://hpln.hpe.com/contentoffering/community-devops-content) .

**Important Note**: HP-OO Chef Content Pack only supports **Windows** knife hosts (learn-chef **chef-mgmt-win** Workstation), HP-OO learn-chef Content Pack too

## Requirements

+ [learn-chef] (https://github.com/gilleslabs/learn-chef) Chef Server [environment] (https://github.com/gilleslabs/learn-chef/blob/master/chef-server.md) up and running. Tested on 1.1
+ [HP Operations Orchestration] (https://hub.docker.com/r/hpsoftware/ooce/). Tested on 10.5
+ HP Operations Orchestration Studio. Tested on 10.5
+ [HP Operations Orchestration Base Content Pack] (https://hpln.hpe.com/contentoffering/oo-base-content) . Tested on 1.6.2  

**Note :** **HP Operations Orchestration Studio** and **HP Operations Orchestration Base Content Pack** are included with **HP Operations Orchestration**

## Available Flows



## Installation

####Getting started:

a. If not already done, install learn-chef :
```
git clone https://github.com/gilleslabs/learn-chef
cd learn-chef
```

b. If not already done, launch Chef Server environment (Chef Server + Windows 2012R2 Workstation + Node)

`vagrant up chef-server node chef-mgmt-win`

**Important note**: 
+ By default **chef-mgmt-win** VM Windows Firewall is enabled.
+ HP-OO learn-chef content pack relies on RPC to pass instruction to chef-mgmt-win VM, **please ensure to allow RPC traffic in Windows firewall rules** 
+ For the sake of simplicity you can also simply disable Windows Firewall on chef-mgmt-win VM.


####Import learn-chef project in HP-OO Studio

1. Download learn-chef-hpoo-content pack [source code] (https://github.com/gilleslabs/learn-chef-hpoo-content-pack/releases)
2. Extract the **learn-chef** folder contained in the source code archive into your HP-OO Studio Workspace folder(usually in C:\users\username\.oo\Workspace)
3. In HP-OO Menu Toolbar:
+ Click on **File**
+ Then click on **Import Project**
+ Browse and select **learn-chef** folder in your HP-OO Studio Workplace folder


## Credits

This project was totally inspired from [HP OO DevOps Content Pack](https://hpln.hpe.com/contentoffering/community-devops-content)

## Copyright

