# ☁ Cloud Attack Defense Homelab
Deploy an attack/defend cybersecurity homelab.

# Architecture 
Provider: AWS.

![image](https://github.com/user-attachments/assets/745396ea-435d-429c-9c51-d3e269f4d7ed)


# Download 
`git clone https://github.com/Poatan222/Cloud-Attack-Defense-Lab.git`

`cd Cloud-Attack-Defense-Lab`

# Deploy [Infrastructure Deployment Steps:]

The entire repository is deployed using terraform from hashicorp. It will spin up the required resources as mentioned in the architecture diagram. while this is basic plan to perform attack and defense; feel free to experiment the changes in the given architecture. 

`terraform init`: Initialize Terraform.

`terraform plan`: Plan Terraform configuration. (Will load the requried terraform files)

`terraform apply -var="aws-key"`: Specify the public key name created in AWS in EC2 -> Network & Security.
- Add Public Key Name in between double quotes.
Note: Replace "your-key-name" with your AWS EC2 key pair name

`terraform destory`: # Remove all the created resources.
