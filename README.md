# TF AWS Layout Generator

## overall
* tf generates a `dot` format file showing layout
* `dot` format file uses dot to generate diagram
* example command: `terraform graph | dot -Tsvg > graph.svg`

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
        * Missing
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

## Layout Notes

* Region: Outermost box, solid black line, transparent background, "AWS" logo in upper left, rounded corners, usually says "Region" at bottom. Not sure how multi-region diagrams look, initially only support one region.

* VPC: Second most outermost box, solid black line, transparent background, "VPC" logo in upper left, rounded corners.

* VPC Peering: Double-line joining the VPC boxes with VPC Peering icon in middle of line

* Availability Zone: Orange dashed line box with light semi-transparent orange background. Name (ex. 'Availability Zone 1') in orange centered left to right, above bottom line of AZ box. If stacked vertically, left-right edges extend outside VPC box. If stacked horizontally, top-bottom edges extend outside VPC box. 

* Subnet: Entirely within VPC box, lock icon in upper left, solid black line, transparent background. Public subnets have light green background, Private subnets have a light blue background. Subnet name and CIDR centered left to right, above bottom line.

* EC2 Instance: Orange box EC2 icon, Name in black text centered left to right and below box.



