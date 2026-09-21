# S3 Configuration

## Purpose

The purpose of this section is to document the configuration of the Amazon S3 bucket used for my static website.

## Bucket

The project uses an Amazon S3 bucket to store the static website files.

### Website Files

The bucket contains:

* `index.html`
* `style.css`

## AWS Region

The bucket is located in:

```text
[United States (N. Virginia)]
```

## Static Website Hosting

Static website hosting is enabled.

The index document is:

```text
index.html
```

## Object Storage

The website files are stored as objects inside the S3 bucket.

The main objects are:

```text
index.html
style.css
```

## Access Configuration

The current Block Public Access configuration is:

```text
[All public access is blocked]
```

The current bucket policy configuration is:

```text
[Public access is blocked because Block Public Access settings are turned on for this bucket]
```

## Object Ownership

The current Object Ownership setting is:

```text
[ACLs disabled]
```

## What I Learned

I learned that an S3 bucket contains objects and that bucket-level configuration controls how those objects are managed and accessed.

I also learned that static website hosting and access permissions are separate configuration areas.

## Security Considerations

S3 access configuration needs to be handled carefully because incorrect permissions can expose stored objects to unintended users.

I will investigate the security implications of the current configuration in the next step.

## Next Step

The next step will focus on security considerations for the S3 deployment.
