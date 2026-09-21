# Cloud Deployment Results

## Objective

The objective of this project was to deploy a simple static website to Amazon S3 and understand the basic concepts involved in cloud storage, website hosting and access control.

## Deployment

The website was deployed using an Amazon S3 bucket.

The deployment process included:

1. Creating an S3 bucket.
2. Uploading the website files.
3. Enabling static website hosting.
4. Configuring public access for the website objects.
5. Creating a bucket policy allowing public read access.
6. Testing the website through the S3 website endpoint.

## Website Files

The bucket contains the following website files:

* `index.html`
* `style.css`

## Access Configuration

The S3 website required public read access because the website is being served directly through the S3 static website endpoint.

A bucket policy was used to allow:

```text
s3:GetObject
```

for the website objects.

## Testing

The website was tested using the S3 website endpoint.

The test confirmed that:

* The website loads successfully.
* The HTML content is displayed.
* The CSS styling loads correctly.
* The website files are accessible through the S3 website endpoint.

## Security Considerations

Because the website objects are publicly accessible, sensitive information must never be stored in the bucket.

The project demonstrates public S3 website hosting for learning purposes.

For a production website, a more secure architecture could use Amazon CloudFront with an S3 bucket rather than exposing the S3 website endpoint directly.

## What I Learned

Through this project I learned:

* What cloud storage is.
* How Amazon S3 buckets and objects work.
* How static websites can be hosted using S3.
* How AWS regions affect resources.
* How bucket policies control access.
* How public access settings affect S3 websites.
* How to test a cloud deployment.
* Why security must be considered when making resources publicly accessible.

## Conclusion

The static website was successfully deployed and tested using Amazon S3.

The project provided practical experience with AWS storage, static website hosting, access control and basic cloud security.
