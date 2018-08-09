# TF AWS Layout Generator

## overall
* tf generates a `dot` format file showing layout
* `dot` format file uses dot to generate diagram

## icons
* simple icons page: https://aws.amazon.com/architecture/icons/
* direct link: https://s3-us-west-2.amazonaws.com/awswebanddesign/Architecture+Icons/AWS-Arch-Icon-Sets_Feb-18/PNG%2C+SVG%2C+EPS_18.02.22.zip
* unzip


* display image in dot file layout: https://stackoverflow.com/questions/8073115/how-do-i-get-dot-to-display-an-image-for-a-node

* Icons used (in 'PNG, SVG, EPS' folder)
    * VPC
        * ..\General\General_virtualprivatecloud.png
        * ..\Compute\Compute_AmazonVPC.png
    * RDS 
        * ..\Database\Database_AmazonRDS.png
    * WAF
        * ..\Security Identity & Compliance\SecurityIdentityCompliance_AWSWAF.png
    * Route Table
    * Subnet
    * Security Group
    * EC2 Instance
        * ..\Compute\Compute_AmazonEC2_instance.png
    * Application Load Balancer
        * ..\Networking & Content Delivery\NetworkingContentDelivery_ElasticLoadBalancing_ApplicationLoadBalancer.png  
        * ..\Compute\Compute_ElasticLoadBalancing_ApplicationLoadBalancer.png
    * NAT Gateway
        * ..\Networking & Content Delivery\NetworkingContentDelivery_ElasticLoadBalancing_ApplicationLoadBalancer.png
        * ..\Compute\Compute_AmazonVPC_VPCNATgateway.png
    * Internet Gateway
        * ..\Compute\Compute_AmazonVPC_Internetgateway.png
    * VPC Peering
        * ..\Networking & Content Delivery\NetworkingContentDelivery_AmazonVPC_VPCpeering.png
        * ..\Compute\Compute_AmazonVPC_VPCpeering.png
    * Router
        * ..\Networking & Content Delivery\NetworkingContentDelivery_AmazonVPC_router.png