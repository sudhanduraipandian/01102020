# 02162021
## aws_ec2_wordpress

### Step 1:
Login to AWS Management console and select EC2 from the compute services.

### Step 2:
Click on "Launch Instance" button. There are multiple options to host a wordpress application using AWS EC2 insstance. The easiest way is to launch a EC2 instance which is readily available with most of our requirement.

### Step 3:
Search for the term "wordpress". We can see multiple options available under the categories "AWS Marketplace" and "Community AMIs"

### Step 4:
This is the actual STEP 1 in the process. Select the image "WordPress Certified by Bitnami and Automattic" under AWS Marketplace which is eligible for free tire. There are multiple options available under free tire we can choose which is more suitable for our requirement. After selecting the required image, we can see a page which lists all the available instance types with the cost.

### Step 5:
Click on "Continue" to select the type of instance required. *t2.micro* is eligible for free tire which includes 1 virutal CPU unit, 1 GiB memory. This type of instance can be used only with a EBS storage volume, suitable for moderate network performance and supports IPv6.

### Step 6:
After selecting the instance type we can skip all other steps and choose to review and launch the instance at any moment or Click on "Next:Configure Instance Details" to configure the Number of instances, Network, IAM role, etc,. 

### Step 7:
On the next step, we can add a storage for the instance where we can choose the type of volume and storage size. Also we can choose to keep or delete the volume when the instance is terminated.

### Step 8:
Next step is to add tags to the instance which is used to identify the instance. Eg- Name. A maximum of 50 tags can be added to a EC2 instance.

### step 9:
Now we must add a security group to the instance. We can create a new one or select one from the available list if there is any. While creating a new security group, we can add rules for the type of access we provide to the instance such as SSH, HTTP, HTTPS, etc., and define a protocol, Port, and source each type.

### Step 10:
On clicking the "Review and Launch" button we can Review AMI details, Instance type, Security groups, Instance details, Storage volumes and Tags. If there is any changes to be made, we can go back to the particular stage and do the changes before launching the instance.

### Step 11:
Once all the review is done, Click on "Launch". There will be pop-up where we can selece an existing key pair or create a new one or launch the instance without a key pair. A key pair consists of a public key that AWS stores, and a private key file that you store. Together, they allow you to connect to your instance securely. For Windows AMIs, the private key file is required to obtain the password used to log into your instance. For Linux AMIs, the private key file allows you to securely SSH into your instance. The selected key pair will be added to the set of keys authorized for this instance. To create a new Key pair, just enter the name of the keypair and download the .pem file. You have to download the private key file (.pem file) before you can continue. Store it in a secure and accessible location. You will not be able to download the file again after it's created Key pairs can also be added or removed after launching the instance.

### *We can find our instance on the list of running instances from the EC2 dashboard.*
