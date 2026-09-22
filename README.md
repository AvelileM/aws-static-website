# AWS Static Website

**WTC Project ID:** WTC-QWU35XF7

## About

This is my Cloud Computing solo project for WeThinkCode_.

The project demonstrates the basic process of creating a static website and deploying it to Amazon Web Services (AWS) using Amazon S3.

The project focuses on practical cloud fundamentals, deployment, access control, security considerations and testing.

## Project Goals

* Understand basic cloud computing concepts
* Learn the fundamentals of AWS
* Understand Amazon S3
* Create and deploy a static website
* Learn about cloud access control and permissions
* Apply basic security principles
* Test and document a cloud deployment

## Technologies

* HTML
* CSS
* AWS
* Amazon S3
* Git
* GitHub

## Architecture

The basic deployment flow is:

```text
Local Computer
      |
      v
   GitHub
      |
      v
  Amazon S3
      |
      v
Static Website
```

The website files are stored as objects in an Amazon S3 bucket and served through the S3 static website endpoint.

## Project Structure

```text
aws-static-website/
│
├── README.md
├── index.html
├── style.css
│
├── 02-aws-learning/
│   └── README.md
│
├── 03-deployment-plan/
│   └── README.md
│
├── 04-s3-deployment/
│   └── README.md
│
├── 05-s3-configuration/
│   └── README.md
│
├── 06-security-considerations/
│   └── README.md
│
├── 07-testing/
│   └── README.md
│
└── 08-deployment-results/
    └── README.md
```

## Project Work

### 1. AWS Learning

I investigated basic AWS concepts including:

* Cloud computing
* AWS Regions
* Amazon S3
* S3 buckets
* S3 objects
* Static website hosting

### 2. Website Development

I created a simple static website using HTML and CSS.

The website consists of:

* `index.html`
* `style.css`

### 3. Deployment Planning

I created a deployment plan describing how the website would be moved from my local computer to Amazon S3.

### 4. S3 Deployment

I created an S3 bucket and uploaded the website files.

Static website hosting was enabled with `index.html` configured as the index document.

### 5. S3 Configuration

I investigated:

* Bucket region
* Website hosting configuration
* Objects
* Block Public Access
* Object Ownership
* Bucket permissions

### 6. Security

I investigated the security implications of making website objects publicly accessible.

The project uses public read access because the website is being served directly through the S3 static website endpoint.

No passwords, API keys, credentials or other sensitive information are stored in the bucket.

### 7. Testing

The deployed website was tested through the S3 website endpoint.

Testing confirmed that:

* The website loads successfully.
* `index.html` is displayed.
* `style.css` loads correctly.
* The required website objects are available.

## What I Learned

Through this project I learned:

* Basic cloud computing concepts
* AWS fundamentals
* How S3 buckets and objects work
* How static websites can be hosted using S3
* How access permissions affect cloud resources
* Basic cloud security considerations
* How to test a cloud deployment
* How to document technical work using Git and GitHub

## Security Considerations

The website bucket contains only public website files.

Sensitive information should never be stored in a publicly accessible S3 bucket.

For a production website, a more secure architecture could use Amazon CloudFront with an S3 bucket rather than relying directly on the S3 website endpoint.

## Future Improvements

Possible future improvements include:

* Using Amazon CloudFront
* Using HTTPS through a production cloud architecture
* Adding a custom domain
* Automating deployment using CI/CD
* Managing infrastructure using Infrastructure as Code

These improvements are outside the scope of this beginner project.

## Project Status

**Completed**

The website has been deployed, tested and documented using Amazon S3.

## Learning Approach

The project was developed incrementally.

For each stage I:

1. Investigated the concept.
2. Applied it practically.
3. Observed the result.
4. Documented what I learned.
5. Committed the changes using Git.

This approach helped me understand the concepts rather than simply following deployment instructions.
