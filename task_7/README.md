# DareIT - cloud_challenge
# 7. CI/CD

Knowledge Base: 
CI/CD - Ciągła Integracja (Continuous Integration, CI) i Ciągłe Dostarczanie (Continuous Delivery, CD), continuous integration and continuous deployment (CI/CD) pipeline,
Software Development Life Cycle (SDLC), trigger.

TASK 7
We will now create a CI/CD pipeline using GitHub Actions.

Step 1
Create a Service Account for Terraform. Go to IAM in the GCP Console.

Step 2
Let’s create a bucket in which we will store the terraform state file. Do not grant public access to this bucket.

Step 3️
Create a new repository in Github e.g. dareit-terraform . Go to the Settings tab in the repository. Choose Actions under the Security section. Click the button New repository secret.
Paste the contents of the your-file-name.json that we modified in Step 1. Name the secret TF_GOOGLE_CREDENTIALS . We will later refer to the name of that variable in our Pipeline.
Download the repository to your local.

Step 4
Let’s prepare our code. In Task 6 we put whole terraform code into one main.tf, now we will make it a bit nicer.
- Create file backend.tf (remember to provide the name of the bucket you create in Step 2)
- Create file provider.tf (remember to input the right project id)
- Create main.tf

Step 5
Time for the most important bit. The file with the definition of the pipeline.
We will want the pipeline to run every time we push a new commit to the main branch in our repository.
The pipeline has a few steps:
Checkout
Setup Terraform
Terraform Init
Terraform Formt
Terraform Plan
Terraform Apply

Step 6
Now commit all files to the repo and push the change to the remote repository. Go to github.com and check the Actions tab in your repository. You should see the workflows in there (in other tools e.g gitlab we would call them pipeline runs).

Step 7
1. Modify the workflow so that the job will only be triggered whenever a new pull request is opened.
2. Create a branch called feat/add-bucket
3. On your branch, modify the code of the main.tf to add a new bucket.
4. Open a pull request.
