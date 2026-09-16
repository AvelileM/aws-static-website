# AWS Static Website Deployment Plan

## Project Goal

The goal of this project is to deploy a simple static website using Amazon S3.

The website currently consists of HTML and CSS files.

## Planned Architecture

```text
Local Computer
      |
      | HTML + CSS files
      v
   Amazon S3
      |
      | Static website hosting
      v
   Web Browser
```

## Deployment Components

### Local Computer

I will develop and test the website locally before deploying it.

The current website contains:

* `index.html`
* `style.css`

### Amazon S3

I plan to create an S3 bucket to store the website files.

The bucket will contain the objects required by the static website.

### Web Browser

After deployment, a web browser will be used to access the website.

## Planned Deployment Process

1. Create an S3 bucket.
2. Choose an appropriate AWS Region.
3. Upload the website files.
4. Configure the bucket for static website hosting.
5. Configure the required access settings.
6. Test the website.
7. Document the configuration.
8. Review security considerations.

## Why S3?

S3 is suitable for this project because the website is static.

The website does not require a server-side application or database to generate its pages.

The HTML and CSS files can be stored as objects and served to visitors.

## Security Considerations

During deployment I will investigate:

* S3 bucket access
* Public versus private access
* Least-privilege access
* Protection against unintended access
* Whether the website files are accessible as intended

I will document the final security configuration after deployment.

## Current Status

The website has been created locally and styled with CSS.

AWS deployment has not yet been performed.

## Next Step

The next step will be to create the S3 bucket and begin the website deployment.
