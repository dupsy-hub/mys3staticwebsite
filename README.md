🚀 Set Up Static Website Hosting on AWS S3 Using Terraform
🧰 Prerequisites
An active AWS account
Terraform installed on your local machine

📁 Project Structure
bash
Copy
Edit
.
├── .gitignore              # Ignore Terraform state files and credentials
├── README.md               # Project documentation
├── error.html              # Custom error page
├── index.html              # Main static site page
├── main.tf                 # Main Terraform config to create S3 bucket and settings
├── outputs.tf              # Outputs S3 website URL
├── provider.tf             # AWS provider configuration
├── variables.tf            # Input variables

📋 Overview
This project automates the setup of a static website hosted on AWS S3 using Terraform. It includes bucket creation, website hosting configuration, access settings, and file upload instructions.

🛠️ Steps
Create an S3 Bucket
Terraform will create an S3 bucket with a globally unique name to host your website files.

Configure for Static Website Hosting
The bucket will be configured to host a static website by enabling the feature and specifying:

index.html as the default document

(Optional) error.html for error handling

Upload Website Files
Upload your static assets (HTML, CSS, JS, images) to the S3 bucket. Files will be made publicly accessible using proper ACLs or bucket policies.

Enable Public Access
A bucket policy will be applied to allow public read access so users can view your site without authentication.

Test the Website
Access your hosted site via the S3 static website endpoint or configure a custom domain using Route 53 (optional).

🚀 Bonus
This entire setup — including bucket creation, website configuration, and permissions — is managed with Terraform, allowing for fast deployment and easy teardown.

