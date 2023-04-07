# DareIT - cloud_challenge
# 6. Infrastructure as a Code

Task 6 point 4 - Copy the URL of the object (index.htm) from your bucket and add it to readme.md.
https://console.cloud.google.com/storage/browser/patrycjas-unique-name-of-bucket


Knowledge Base: HashiCorp Terraform, Infrastructure as Code (IaC), Configuration Management, Application Programming Interface (API).

TOOLS: 
- Google Cloud Platform
- Terraform

TASK 6
We will now create some basic resources using Terraform. And to make it nice and easy let’s benefit from the fact the Cloud Shell has preinstalled Terraform.

Step 1
Open Cloud Shell and check the version of Terraform.

Step 2
Create a file called main.tf
We will try to create Compute Instance using terraform. Let’s check out the documentation by Terraform.

Step 3️
As part of this task create a few resources using terraform.
1. Create main.tf file, configure the provider and add configuration to create resources: 
- Cloud Storage bucket that has public access configured
- Compute Instance
- Cloud SQL instance with Postgres engine. Create database called dareit and a user called dareit_user
2. Manually change the password of the dareit_user
3. Upload manually the index.html file (that you previously created in Task 1) into the newly created bucket.
4. Create a new folder in your cloud_challenge repo with name task_6 , commit the main.tf file there. (don’t commit your terraform state file). Copy the URL of the object (index.htm) from your bucket and add it to readme.md.
My answer:
https://console.cloud.google.com/storage/browser/patrycjas-unique-name-of-bucket

Step 4 OPTIONAL
You can install terraform locally on your machine. And use Service Account for credentials.
