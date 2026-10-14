# AWS S3 Static Website Hosting

## Project Overview
This project demonstrates how to host a static website using Amazon Simple Storage Service (Amazon S3) as part of the Week 2 Cloud Computing internship assignment.

## Objective
To store website files in an S3 bucket, enable static website hosting, configure public read access for the website objects, and verify the website through the S3 website endpoint.

## AWS Service Used
- **Amazon S3:** Stores the website files and serves the static website.

## Website Files
The S3 bucket contains these files:
- `index.html` — the main homepage.
- `style.css` — styles the website.
- `error.html` — the error page configured for website hosting.

## Implementation Steps
1. Created an S3 bucket named `manish-static-site-111026` in the Asia Pacific (Mumbai) Region (`ap-south-1`).
2. Uploaded `index.html`, `style.css`, and `error.html` to the bucket.
3. Enabled **Static website hosting** in the bucket's Properties tab.
4. Configured `index.html` as the index document and `error.html` as the error document.
5. Added a bucket policy granting `s3:GetObject` permission for the website objects so visitors can read the files.
6. Opened the S3 website endpoint in a browser and verified that the website loaded successfully.

## Live Website
[Open the S3 static website](http://manish-static-site-111026.s3-website.ap-south-1.amazonaws.com)

**Note:** This endpoint is available only while the bucket exists and its hosting configuration and access permissions remain in place.

## Result
The static website was successfully hosted using Amazon S3 and tested through the S3 website endpoint.

## Screenshots and Evidence
Add the task screenshots to the repository, for example:
- S3 bucket overview
- Uploaded website files
- Static website hosting configuration
- Bucket policy
- Live website in a browser

## Optional Enhancements
CloudFront distribution and a custom domain using Route 53 were optional extensions in the assignment and were not required for the basic S3 static website hosting task.
