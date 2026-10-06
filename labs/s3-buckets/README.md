# S3 Bucket Security

For the bootcamp I built a presentation on how S3 buckets get exposed and how to lock them down. I made up a company, CloudForge Security, to present it.

## What I covered
- What S3 is, and how a misconfigured bucket can leak data
- IAM policies and the difference between managed and inline policies
- How ACLs can make a bucket or object public
- Best practices: block public access, review policies, encrypt data, and turn on AWS Config

## What I tested
- Turned on Block All Public Access and confirmed a request to the bucket returned Access Denied.
- Changed the ACL to allow public listing and confirmed a file was then reachable from outside the account.
- Used the AWS CLI to list the bucket and curl to request a file.

## Takeaway
One setting can be the difference between private and public. If I saw an alert about a public bucket in a SOC, this is the first thing I'd check.

[View the slides (PDF)](s3-bucket-presentation.pdf)
