**Tutorial Link :**

**https://dev.to/goodidea/how-to-fake-aws-locally-with-localstack-27me**
1. Install Docker
2. Install AWS CLI
3. aws configure to create credentials






**Notes**
1. To check whether service is running or not _localhost:4566_
2. Create a bucket: aws --endpoint-url=http://localhost:4566 s3 mb s3://demo-bucket
3. Attach an ACL to the bucket so it is readable: aws --endpoint-url=http://localhost:4566 s3api put-bucket-acl --bucket demo-bucket --acl public-read
4. To check the api calls go to .localstack/data/recorded_api_calls.json
