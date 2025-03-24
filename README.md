Set Up a Static Website Hosting on AWS S3 Bucket

Prerequisite:
1.	AWS account
2.	Terraform installed

Steps:
1.	Create an S3 bucket: Start by creating an s3 Bucket to store your website files. The bucket name should be globally unique across all AWS accounts
2.	Configure Bucket for Static Website Hosting: In the s3 bucket properties, enable static website and specify the default index document (e.g., index.html) and optional error document (e.g., error.html)
3.	Upload Website Files:  Upload your static website files (HTML, CSS, JS images etc.) to the s3 bucket, setting up appropriate permissions e.g., public-read, for objects to be publicly accessible.
4.	Enable Public Access: Allow public access to the s3 bucket and its objects by configuring the bucket policy and ACLs.
5.	Testing the Website: Once the setup is done., you can test the website by accessing it through s3 bucket website URL or your custom domain.

The above steps will be automated using Terraform.
