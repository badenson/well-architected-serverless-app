# Security Considerations

## IAM Roles

- Each Lambda function has its own IAM role
- Roles follow principle of least privilege
- DynamoDB access controlled with fine-grained policies

## API Security

- API Gateway uses JWT authentication via Cognito
- Rate limiting enabled on API endpoints
- Input validation in Lambda functions

## Data Security

- DynamoDB tables encrypted at rest
- Sensitive data encrypted in transit (TLS 1.2+)
- Audit logging enabled for all AWS services

## Monitoring

- CloudWatch alarms for abnormal activity
- AWS Config rules for compliance monitoring
- Regular security reviews of IAM policies