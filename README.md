# Project Overview
Serverless image processing application enables users to upload images to an S3 bucket via API Gateway, triggering an AWS Lambda function that processes and resizes the images before storing them in another S3 bucket, and triggering another AWS Lambda function that saves images metadata into an Amazon DynamoDB.
# Key AWS Services Used:
- **AWS CloudFormation:** For Managing infrastructure as a code, and providing disaster recovery capabilities.
- **Amazon S3:** Used s3 bucket for storing original images, and one for processed images.
- **Amazon API Gateway:** Expose an API for uploads.
- **AWS Lambda:** Handles API requests and performs image processing before storing in another S3 bucket.
- **AWS IAM:** For managing access control via roles and permissions.

# Key Features:
- **Serverless Architecture:** Entirely built on AWS serverless services, enabling auto-scaling.
- **Event-Driven Architecture:** Lambda functions are triggered only when needed - API request, or S3 bucket addition event - , reducing costs.
- **Cost-Effectiveness:** Pay only for usage with no need for managing infrastructure.
- **Metadata tracking:** Storing metadata for all uploaded images into DynamoDB.
- **Scalability:** Automatically handles traffic spikes without performance reduction.
- **Security:** AWS IAM provides fine-grained access control.
- **IaaC:** Providing reusability and disaster recovery capabilities.

# Architecture Diagram
![Architecture Diagram](./AWS_Serverless_Image_processing_S3_APIGateway_Lambda_SystemDesign.png
)

# CloudFormation Diagram
![CloudFormation Diagram](./AWS_Serverless_Image_processing_S3_APIGateway_Lambda_CloudFormation.png
)
