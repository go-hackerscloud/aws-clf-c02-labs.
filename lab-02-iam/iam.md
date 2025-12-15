# Objective: Understand IAM concepts by creating a user with limited permissions and best practices.

## Prerequisites: AWS account with root access.

### Steps:

1. Sign in as the root user (or use an IAM user with admin privileges temporarily).
2. Open IAM service → Users → Add user.
3. Create a user named lab-user with programmatic access and AWS Management Console access (optional).
4. Attach a basic policy (e.g., AmazonS3ReadOnlyAccess) or create a custom policy that allows read-only access to S3.
5. Complete the creation and take note of the access key/secret key (if programmatic access chosen; store securely).
6. Sign in with the new user to verify permissions.


## Expected Results:

New IAM user exists with limited permissions.
User can perform only allowed actions (e.g., list S3 buckets if read-only policy applied).
Assessment / Checklist:

## IAM user created
 Appropriate permissions applied (least privilege)
 Access keys stored securely (if used)

##  Assessment / Checklist:

1. IAM user created
2. Appropriate permissions applied (least privilege)
3. Access keys stored securely (if used)
