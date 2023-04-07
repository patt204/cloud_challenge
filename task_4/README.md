# DareIT - cloud_challenge
# 4. Create Virtual Machine

Knowledge Base (Server rack, Computer Network, Compute Engine, Ethernet, Wi-Fi, Carrier, Bandwidth, Collision domain, Internet, Routing, Router, IP address, virtual machine (VM), web server, virtual private cloud (VPC), subnet or subnetwork, vCPU, firewall ).

TASK 4
You will now learn how to create one of the most basic components used in the Cloud - a Virtual Machine.

Step 1
Go to Google Console. Choose Compute Engine from the Navigation Menu, then VM Instances. Choose CREATE INSTANCE.

Step 2
Now you will be able to to create a Virtual Machine Instance. Type in the name of your virtual machine instance. Choose a region. The region indicated in what data centers the virtual machine will be created.

Step 3️
So far we specified the instance type, name, region. Now we need to decide who can access the VM instance. Keep the default service account.

Step 4 
In the Firewall section mark both HTTPs and HTTP.

Step 5
Click Advanced options. And then Networking. Add a network tag dareit-public . This tag will be used to match firewall rules to the instances to which the rules should apply.

Step 6
Now we can choose Network. Click on the Network, you will see more options. Choose subnetwork. As well as decide whether our instance should get a public IP address (External IPv4 address), so address that is globally unique over the public Internet.

Step 7
Now we will connect to the Virtual Machine Instance. Click on the SSH button in the Connect column.

Step 8
In this step you will:
- get package information from all configured sources (sudo apt update) and install the     Apache Web server (sudo apt -y install apache2)
- we will check the status of the Apache server (we want to see if it is active and running nicely)
- we will remove the preconfigured index.html file
- we will add our own index.html file
So let’s run first the below command in the Terminal. You can copy and paste and hit enter.

Step 9
Copy thet public IP address of your instance and paste it into this form. No Github this time!