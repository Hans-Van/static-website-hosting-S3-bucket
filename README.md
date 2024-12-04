# Hosting A Static Website Using Amazon S3

## Project Overview
This project demonstrates how to host a static website using Amazon S3 (Simple Storage services). The goal is to creat an S3 bucket, uploaded website files, enabled static website hosting, and controlled permissions to make the site public. This guide goes over each step in detail.

## Project Prerequisites
- AWS Account
- IAM user with sufficient permissions

### Table of Contents
1. [About Amazon S3](#about-amazon-s3)
2. [Project Setup](#project-setup-instructions)
   - [Create an S3 Bucket](#create-an-s3-bucket)
   - [Upload Website Files](#upload-website-files)
   - [Enable Static Website Hosting](#enable-static-website-hosting)
   - [Adjust Permissions](#adjust-permissions)
3. [Troubleshooting](#troubleshooting)
4. [Additional Resources](#additional-resources)

   --

## About Amazon S3
Amazon S3 simplifies data storage and management while offering flexibility, security, and global accessibility, making it ideal for businesses and developers.

## Project Setup Instructions

### Step 1: Create an S3 Bucket
   - Go to the [AWS S3 Console](https://aws.amazon.com/s3/).
   - Create a new bucket with a globally unique name.
   - For this project, we used the **EU North (Stockholm)** region (`eu-north-1`), but you can select a region that best suits your needs.

### Step 2. Upload Website Files
   - Upload your `index.html` and other necessary assets (e.g., images or stylesheets) to the S3 bucket.
   - Ensure all assets are correctly referenced in the `index.html` file for smooth loading.

### Step 3. Enable Static Website Hosting
   - Go to the **Properties** tab of your S3 bucket.
   - Under **Static website hosting**, select **Enable** and specify the `index.html` as the default document.
   - Save your changes.

### Step 4. Adjust Permissions
   - To make the website publicly accessible, navigate to the **Permissions** tab.
   - Disable the "Block all public access" setting if necessary.
   - Update the bucket's Access Control List (ACL) to allow public access to the contents.

## Troubleshooting
   - If you see a "403 Forbidden" error when accessing the bucket's endpoint URL, check the following:
   - Ensure public access is enabled.
   - Verify that permissions are correctly set for the bucket and its objects.
   - Confirm that your `index.html` file is properly named and accessible.

## Additional Resources
The PDF paper provided in this repository provides a detailed step-by-step guide with screenshots.

### Credits
This project was completed with the support of the NextWork community, a fantastic resource for hands-on learning in cloud and tech skills. Visit [NextWork](https://community.nextwork.org) for more information.
