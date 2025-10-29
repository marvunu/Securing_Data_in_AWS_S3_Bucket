# Securing_Data_in_AWS_S3_Bucket


<h2>Description</h2>
Created and secured an AWS S3 bucket to manage and protect stored data. Applied best practices by enabling versioning, configuring server-side encryption, setting custom IAM and bucket policies, and activating access logs to ensure visibility and compliance.

<br />

<h2>Environments Used </h2>

- <b>Platform: Amaazon Web Sevice</b>

- <b>AWS Management Console</b>

- <b>Amazon S3</b>

- <b>JavaScript Object Notation </b>

<h2>Project walk-through:</h2>

<p align="center">
 Logged in to the AWS Management Console, navigated to the S3 Dashboard, and created a new bucket named “my-dem0-cucket” in a selected region while ensuring “Block all public access” was enabled to prevent unauthorized users from accessing or exposing stored data.
 <br/>
<img src="https://i.imgur.com/tf8oMsq.png" height="80%" width="80%" alt="S3bucket"/>
  <img src="https://i.imgur.com/ZYqcCkb.png" height="80%" width="80%" alt="S3bucket"/>
<br />
<br />
 Enabled Bucket Versioning to maintain previous versions of objects, ensuring data recovery and protection against accidental deletion or overwrites.

  <br/>
<img src="https://i.imgur.com/Vow3Flt.png" height="80%" width="80%" alt="S3bucket"/>


<br />
<br />
Enabled server-side encryption using AWS KMS, choosing or creating a KMS key to ensure all stored data is automatically encrypted at rest for enhanced security and compliance. <br/>
<img src="https://i.imgur.com/9aXeL9y.png" height="80%" width="80%" alt="S3bucket"/>

<br />
<br />
Added a bucket policy that grants read-only access (GetObject) to the root user identified by their ARN. This policy ensures that only the designated root user can view or download objects from the bucket, maintaining controlled and auditable access to stored data.  It does not allow uploading, deleting, or listing objects. <br/>
<img src="https://i.imgur.com/MRBHCVt.png" height="80%" width="80%" alt="S3bucket"/>
<img src="https://i.imgur.com/5EdqUsr.png" height="80%" width="80%" alt="S3bucket"/>
<br />
<br />
Enabled Server Access Logging, specifying the target bucket to store log files. This configuration ensures that all access requests made to “my-dem0-cucket” are recorded for monitoring, auditing, and troubleshooting purposes.
  <br/>
<img src="https://i.imgur.com/m9X7ub4.png" height="80%" width="80%" alt="S3bucket"/>
<img src="https://i.imgur.com/PXzEMJp.png" height="80%" width="80%" alt="S3bucket"/>



</p>




<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
