---
published: true
---
This second post is about setting up a simple website on AWS.

Step 1: Create a new account or sign into [amazon console](https://aws.amazon.com/console/) using your amazon account

Step 2: Go to the pull down menu for services and select EC2 under compute
![EC2]({{site.baseurl}}/_posts/ec2.PNG)

Step 3: Click on instances to launch a new intsnace using the blue drop down menu

![instance]({{site.baseurl}}/_posts/instance.PNG)

Step 4: New users get certain free accounts to you can select one. I selected the free one for UBUNTU

[instance launch](https://us-west-2.console.aws.amazon.com/ec2/v2/home?region=us-west-2#LaunchInstanceWizard:)

Step 5: select the instance type and select next

![instance type]({{site.baseurl}}/_posts/instance type.PNG)

Step 6: This window will configure instance details. Then click next if you dont need to make any changes. 
![configure Instance]({{site.baseurl}}/_posts/configure_instance1.PNG)

To automatically install a webserver like nginx and git and then dowload your website files from github, copy this script into the User Data Section. Scroll down to the advanced details  
	  
	#!/bin/bash
	sudo apt-get update
	sudo apt-get install nginx git -y
	cd /usr/share/nginx/html/
	sudo rm /usr/share/nginx/html/*
	git clone https://github.com/eshnil2000/test .
    
![User data]({{site.baseurl}}/_posts/configure_instance2_advanced.PNG)


Step 7: Accept the default storage capacity and click next.

Step 8: Create a new security group with ports 80 and 22 open to incoming traffic

Step 9 : To Review and launch
Create a new pair of keys and save the private key. Then click launch.

![launch]({{site.baseurl}}/_posts/launched_instance.PNG)

