# AWSxDevOps
Welcome to this AWSxDevOps project series! In this SEVEN-project series, I will create a CI/CD pipeline to build and deploy a simple web application using AWS' Code services.

## Here's what you'll build at the end of ALL seven projects:

Welcome to this DevOps project! In this guide, you'll learn how to host a static website using Amazon S3, a highly scalable storage service provided by AWS. By the end of this project, you'll have your own website hosted and publicly accessible on the web.

![Project Screenshot](assets/screenshots/s3-website.png)

## ⚡️ 30 Second Summary

**Difficulty**: Easy peasy  
**Time**: 45 min  
**Cost**: $0  
**Tools Needed**:
- An AWS account - [Create one here!](https://aws.amazon.com/free/)

## AWS Services Used

- Amazon S3

## What You'll Achieve

- Create an Amazon S3 bucket.
- Upload website content to the S3 bucket.
- Configure S3 to host a static website.
- Make the website publicly accessible.

## How It Works

1. **Create a Bucket**: Set up an S3 bucket where you'll store your website files.
2. **Upload Content**: Upload your website's HTML files and assets to the bucket.
3. **Configure Static Website Hosting**: Set up your S3 bucket to serve as a static website host.
4. **Make Public**: Configure your bucket's permissions to make the website publicly accessible.

## Project Steps

### Step 1: Create a Bucket in Amazon S3

1. Sign in to the AWS Management Console and navigate to Amazon S3.
2. Click **Create bucket**.
3. Choose a region and enter a globally unique name for your bucket.
4. Enable ACLs (Access Control Lists) to manage permissions.
5. Disable **Block all public access** and confirm the warning.

   ![Bucket Creation](assets/screenshots/bucket-creation.png)

6. Click **Create bucket** to complete the setup.

### Step 2: Upload Website Content

1. Open your new bucket in the S3 console.
2. Click **Upload** and select your website files (`index.html` and other assets).
3. Upload the files and confirm the successful upload.

   ![Upload Content](assets/screenshots/upload-content.png)

### Step 3: Configure Static Website Hosting

1. In your S3 bucket, go to the **Properties** tab.
2. Scroll to the **Static website hosting** section and select **Use this bucket to host a website**.
3. Enter `index.html` as the index document.

   ![Website Hosting](assets/screenshots/website-hosting.png)

4. Save changes and note the bucket website endpoint URL.

### Step 4: Make the Website Public

1. Go back to the **Permissions** tab in your bucket settings.
2. Use ACLs to set the permissions of your files to public.

   ![Make Public](assets/screenshots/make-public.png)

3. Refresh the website endpoint URL to see your live site.

## Deleting Resources

To avoid unnecessary charges, make sure to delete all AWS resources after completing the project:

1. Delete the objects in your bucket.
2. Delete the bucket itself.

## Share Your Work

Share your project on LinkedIn to showcase your achievement! You can use the downloadable documentation as proof of your work.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Let's Connect

Feel free to reach out or follow me for more updates on my journey through AWS and DevOps!

**Happy Hosting!** 🌟
