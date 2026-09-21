# S3 Security Considerations

## Overview

This section documents the security considerations for hosting a static website using Amazon S3.

The purpose is to understand how access controls affect the security of an S3 bucket and its objects.

## Public Access

A static website hosted directly through an S3 website endpoint needs its website files to be publicly accessible.

However, making an S3 bucket public can create security risks if sensitive files are accidentally uploaded.

For this project, the bucket only contains public website files such as:

* `index.html`
* `style.css`

No passwords, API keys, personal information or other sensitive data should be stored in the bucket.

## Block Public Access

Amazon S3 provides Block Public Access settings to help prevent unintended public access to buckets and objects.

These settings should be reviewed before making a bucket publicly accessible.

For this learning project, the Block Public Access configuration was inspected in the AWS Console before changing access settings.

## Bucket Policy

An S3 bucket policy can control who is allowed to access resources in the bucket.

For a public static website, a policy may be required to allow visitors to retrieve website objects.

Any bucket policy should follow the principle of least privilege and only grant the permissions required.

## Sensitive Information

Sensitive information should never be stored in a publicly accessible website bucket.

Examples include:

* Passwords
* API keys
* Access keys
* Private documents
* Database credentials
* Personal information

## Security Lessons

This investigation demonstrated that:

* Public access should be intentional.
* Sensitive information should never be stored in a public bucket.
* S3 permissions should be reviewed carefully.
* Access should follow the principle of least privilege.
* Security settings should be tested after making changes.

## Future Improvement

For a production website, a more secure architecture could use Amazon CloudFront in front of an S3 bucket rather than relying directly on the S3 website endpoint.

This project uses direct S3 static website hosting as a learning exercise to understand AWS storage, hosting and access control.
