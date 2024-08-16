## Virtual Private Cloud (VPC) network on Google Cloud Platform (GCP)

A VPC provides a logically isolated network partition on GCP and offers several features including:

1. Private IP Addressing: Control over IP address range selection and subnet segmentation.
2. Subnets: Divide the VPC network into subnets for better organization and control.
3. Routing: Manage internal and external IP traffic flow with custom routes.
4. Firewall Rules: Define security rules to allow or deny traffic to/from VM instances.
5. Private Connectivity:  Secure communication within and outside GCP via VPN or dedicated interconnects.
## Key Components of a VPC in GCP with Terraform

1. VPC Network: The primary container for subnets, routes, firewall rules, etc.
2. Subnets: Segments of the VPC network, each with its own IP range.
3. Firewall Rules: Security rules to control traffic to/from the VPC network.
4. Routes: Rules that determine how traffic is directed within the VPC.
## Steps to Use Terraform with GCP for VPC network

1. Install Terraform: Download and install Terraform from the official website.

2. Authenticate GCP: Ensure you are authenticated to your GCP project using the gcloud CLI or a service account.

3. Create the Configuration: Write the Terraform configuration file.

4. Initialize Terraform: Initialize the working directory containing the configuration file.

       terraform init
5. Plan the Deployment: Create an execution plan to preview the changes that will be made.

       terraform plan

 6. Apply the Configuration: Apply the changes to create the resources on GCP.
 
        terraform apply

      

## Notes

1. We control all the traffic coming in and going outside a VPC.
2. VPC is a global resource & contains subnets in one or more
region.VPC resources can be in any
region or zone.
## Documentations
1. https://cloud.google.com/vpc/docs/
2. https://registry.terraform.io/providers/hashicorp/google/latest/docs/data-sources/vpc_access_connector
