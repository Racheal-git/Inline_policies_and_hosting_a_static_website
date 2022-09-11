# Inline_policies_and_hosting_a_static_website
Adding inline policy to a user and hosting a static website on AWS

IAM INLINE POLICIES AND HOSTING A STATIC WEBSITE

Inline policy are policies created and managed to be inherited by a specific user example read-only policy for an auditor. Also means, the auditor has access to the console but can only read and has no other access.
To create inline policy:
    • Log into IAM console on AWS, 
    • Go to User and add users
    • Skip the attach permission and add tags. e.g Name – Auditor
    • Create user and click on the user name created 
    • At the right side, click on the inline policy
    • Edit the Jason code to one of read only access code under IAM documentation.
    • Review Policy and Assign the policy to the Auditor.
    • Only the Auditor can inherit this policy.

To host a static website, you need to first create an s3 bucket on AWS

An s3 bucket allows you to upload your files for when ever it is needed.
To create an s3 bucket:
    • Search s3 in the AWS services
    • Select s3 and Create bucket.
    • Name the bucket
    • Assign a region and uncheck “block all public access” for the website to the publicly accessible.
    • Enable server-side encryption.
    • Enable static website hosting.
    • After configuring settings, upload files.
    • Static website should be accessible publicly now.
