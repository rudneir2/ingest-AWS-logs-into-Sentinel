# ingest-AWS-logs-into-Sentinel

## Architecture reference (draft)

![image](https://user-images.githubusercontent.com/97529152/154762225-aec74571-97ca-4a0b-b109-8a28e18ca98b.png)

## step by step

1. create an assumed role
  https://docs.microsoft.com/en-us/azure/sentinel/connect-aws?tabs=s3#configure-an-aws-service-to-export-logs-to-an-s3-bucket
  
2. create a S3
  https://docs.microsoft.com/en-us/azure/sentinel/connect-aws?tabs=s3#configure-an-aws-service-to-export-logs-to-an-s3-bucket
  
3. create a SQS
  https://docs.microsoft.com/en-us/azure/sentinel/connect-aws?tabs=s3#configure-an-aws-service-to-export-logs-to-an-s3-bucket
  
4. add specific policy to S3
  https://github.com/Azure/Azure-Sentinel/blob/master/DataConnectors/AWS-S3/AwsRequiredPolicies.md
	
5. add specific policy to SQS
https://github.com/Azure/Azure-Sentinel/blob/master/DataConnectors/AWS-S3/AwsRequiredPolicies.md
  
6. enable SQS notification on S3
https://docs.aws.amazon.com/AmazonS3/latest/userguide/enable-event-notifications.html
	
7. get assumed role ARN and SQS URL and finish AWS connector setup on Azure portal
  
8. start collection VPC Logs on Azure (see aggregation time on AWS console)
