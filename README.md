# AWS_Three_Tier_WebApp

This repository contains Image Classification project that provides resilliency and high availability built on AWS. It Contains Three Tier
1) Front End
2) Back end
3) Server

The Backend is Connected to a Load Balancer which acts as a master and assign work to the EC2 Instance. It Scales up as the requests increase and scales down
where there are very few requests. It uses SQS Messaging Queue To Communicate between different tier and takes care of Failed mesasges. Lamba Is used to trigger the Instances upon arrival of New Requests.
