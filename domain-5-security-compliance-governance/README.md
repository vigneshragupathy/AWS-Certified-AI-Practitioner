# Domain 5: Security, Compliance, and Governance for AI Solutions (14%)

## Overview
This domain covers security, compliance, and governance requirements for AI/ML workloads on AWS, including the shared responsibility model, data protection, and regulatory compliance.

## Topics Covered

### 1. AWS Shared Responsibility Model for AI/ML

#### AWS Responsibilities (Security OF the Cloud)

##### Infrastructure Security
- Physical security of data centers
- Network infrastructure
- Hardware and facilities
- Managed service operations

##### Service Security
- Service availability and resilience
- Patching and updates of managed services
- Encryption capabilities
- Compliance certifications

#### Customer Responsibilities (Security IN the Cloud)

##### Data Protection
- Data encryption configuration
- Data classification
- Access controls
- Backup and retention

##### Application Security
- Model security
- Endpoint security
- Application code
- API security

##### Identity and Access Management
- User authentication
- Authorization policies
- Credential management
- Access logging

##### Compliance
- Meeting regulatory requirements
- Data residency compliance
- Audit and reporting
- Security best practices

### 2. Identity and Access Management (IAM)

#### IAM Fundamentals

##### Key Concepts
- **Users:** Individual identities
- **Groups:** Collection of users
- **Roles:** Temporary credentials for services/users
- **Policies:** JSON documents defining permissions

##### Best Practices
- Use roles instead of long-term credentials
- Principle of least privilege
- Enable MFA for sensitive operations
- Regular access reviews
- Use IAM policy conditions

#### IAM for AI/ML Services

##### Amazon Bedrock Permissions
```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Action": [
      "bedrock:InvokeModel",
      "bedrock:InvokeModelWithResponseStream"
    ],
    "Resource": "arn:aws:bedrock:*:*:foundation-model/*"
  }]
}
```

##### SageMaker Permissions
- Execution roles for training jobs
- Endpoint access policies
- Notebook instance roles
- Domain user profiles

##### Resource-Based Policies
- S3 bucket policies for data
- KMS key policies for encryption
- Lambda function policies
- API Gateway authorization

#### Service Control Policies (SCPs)
- Organization-wide permission boundaries
- Restrict services in accounts
- Compliance enforcement
- Cost control

### 3. Data Security and Encryption

#### Encryption at Rest

##### AWS KMS (Key Management Service)
- **Customer Managed Keys (CMK):** Full control over keys
- **AWS Managed Keys:** Automatic rotation
- **Key Policies:** Control key access
- **Envelope Encryption:** Encrypt data encryption keys

##### Service Encryption
- **S3:** Server-side encryption (SSE-S3, SSE-KMS, SSE-C)
- **EBS:** Encrypted volumes
- **SageMaker:** Encrypted training data and models
- **Bedrock:** Encrypted model artifacts

#### Encryption in Transit

##### TLS/SSL
- HTTPS for API calls
- TLS 1.2 or higher
- Certificate management (ACM)
- Secure WebSocket connections

##### VPC Endpoints
- Private connectivity to AWS services
- No internet gateway required
- Traffic stays on AWS network
- Interface and gateway endpoints

#### Data Classification

##### Sensitivity Levels
- **Public:** No restrictions
- **Internal:** Company use only
- **Confidential:** Restricted access
- **Highly Confidential:** Strict controls

##### AWS Services for Classification
- **Amazon Macie:** Discover and protect sensitive data in S3
- **AWS Data Exchange:** Secure data sharing
- **Lake Formation:** Data lake security

### 4. Network Security

#### VPC Configuration

##### Network Isolation
- **VPC:** Isolated network environment
- **Subnets:** Public and private subnets
- **Security Groups:** Stateful firewalls
- **NACLs:** Network access control lists

##### AI/ML in VPC
- **SageMaker VPC mode:** Isolate training and inference
- **Bedrock:** Operates within AWS network
- **VPC endpoints:** Private API access

#### API Security

##### API Gateway
- Authentication (IAM, Cognito, Lambda authorizers)
- Rate limiting and throttling
- Request validation
- API keys and usage plans

##### WAF (Web Application Firewall)
- Protect against common exploits
- Rate-based rules
- Geo-blocking
- Custom rules

### 5. Data Governance

#### Data Lifecycle Management

##### Stages
1. **Collection:** Secure data ingestion
2. **Storage:** Encrypted, access-controlled storage
3. **Processing:** Secure compute environments
4. **Sharing:** Controlled access and auditing
5. **Archival:** Long-term storage (Glacier)
6. **Deletion:** Secure data disposal

##### AWS Services
- **S3 Lifecycle Policies:** Automate data transitions
- **S3 Object Lock:** Prevent deletion/modification
- **AWS Backup:** Centralized backup management
- **Data Pipeline:** Orchestrate data workflows

#### Data Lineage

##### What is Data Lineage?
- Track data origin and transformations
- Understand data flow through systems
- Impact analysis for changes
- Compliance and auditing

##### AWS Tools
- **AWS Glue:** Data catalog and lineage
- **Lake Formation:** Data lake governance
- **DataZone:** Data discovery and governance
- **CloudTrail:** Track data access

#### Data Quality

##### Quality Dimensions
- Accuracy
- Completeness
- Consistency
- Timeliness
- Validity

##### AWS Services
- **AWS Glue Data Quality:** Automated data validation
- **SageMaker Data Wrangler:** Data preparation and validation
- **Lake Formation:** Enforce quality rules

### 6. Compliance and Regulations

#### Key Regulations

##### GDPR (General Data Protection Regulation)
- **Scope:** European Union data protection
- **Requirements:**
  - Right to access
  - Right to be forgotten
  - Data portability
  - Consent management
  - Breach notification (72 hours)

##### CCPA (California Consumer Privacy Act)
- **Scope:** California residents
- **Requirements:**
  - Disclosure of data collection
  - Right to delete
  - Opt-out of data selling
  - Non-discrimination

##### HIPAA (Health Insurance Portability and Accountability Act)
- **Scope:** Healthcare data (US)
- **Requirements:**
  - Protected Health Information (PHI) security
  - Access controls
  - Audit logs
  - Business Associate Agreements (BAA)

##### SOC 2 (Service Organization Control)
- Security, availability, processing integrity
- Confidentiality and privacy
- Third-party attestation
- Continuous compliance

##### ISO/IEC 27001
- Information security management
- Risk assessment
- Security controls
- Regular audits

##### PCI DSS (Payment Card Industry)
- Credit card data protection
- Network security requirements
- Access control measures

#### Industry-Specific Regulations
- **Financial Services:** SOX, GLBA, PSD2
- **Government:** FedRAMP, FISMA
- **Education:** FERPA
- **Telecommunications:** CPNI

### 7. AWS Compliance Programs

#### Compliance Resources

##### AWS Artifact
- **Access compliance reports:** SOC, PCI, ISO reports
- **Download agreements:** BAAs, NDAs
- **Self-service portal:** On-demand access
- **Compliance documentation:** Certifications and attestations

##### AWS Compliance Programs
- 140+ certifications and attestations
- Geographic compliance (data residency)
- Industry-specific compliance
- Regular audits and updates

##### AWS Compliance Center
- Resources and guidance
- Compliance best practices
- Service-specific compliance information

#### Service-Specific Compliance

##### HIPAA-Eligible Services
- Amazon Bedrock (with BAA)
- Amazon SageMaker (with BAA)
- S3, RDS, DynamoDB
- Lambda, ECS

##### PCI DSS Compliant Services
- Infrastructure services (EC2, VPC)
- Storage services (S3, EBS)
- Database services (RDS, DynamoDB)
- AI/ML services with proper configuration

### 8. Governance Frameworks

#### AI/ML Governance

##### Model Governance
- **Model Registry:** Track model versions (SageMaker)
- **Model Approval:** Review and approve models
- **Model Monitoring:** Track performance over time
- **Model Retirement:** Deprecate old models

##### Data Governance
- **Data Catalog:** AWS Glue Data Catalog
- **Access Control:** Lake Formation permissions
- **Data Quality:** Validation and monitoring
- **Metadata Management:** Tags and documentation

##### Infrastructure Governance
- **AWS Organizations:** Multi-account management
- **Service Control Policies:** Permission boundaries
- **AWS Config:** Resource compliance
- **CloudFormation:** Infrastructure as code

#### Policy Enforcement

##### AWS Config
- **Config Rules:** Define compliance requirements
- **Conformance Packs:** Pre-packaged rule sets
- **Remediation:** Automatic or manual fixes
- **Compliance Dashboard:** View compliance status

##### AWS Control Tower
- Multi-account governance
- Preventive guardrails (SCPs)
- Detective guardrails (Config rules)
- Account factory
- Centralized compliance

### 9. Audit and Monitoring

#### Logging and Monitoring

##### AWS CloudTrail
- **API Call Logging:** Who did what, when
- **Integration:** CloudWatch, S3, Athena
- **Compliance:** Audit trail for regulations
- **Security Analysis:** Detect anomalies
- **Multi-region and Organization trails**

##### Amazon CloudWatch
- **Metrics:** Performance monitoring
- **Logs:** Application and service logs
- **Alarms:** Automated notifications
- **Dashboards:** Visualization
- **Insights:** Log analysis

##### VPC Flow Logs
- Network traffic monitoring
- Security analysis
- Troubleshooting
- Compliance auditing

#### AI/ML Specific Monitoring

##### SageMaker Model Monitor
- Data quality monitoring
- Model quality monitoring
- Bias drift detection
- Feature attribution drift

##### Bedrock Monitoring
- Model invocations (CloudWatch)
- Latency and errors
- Token usage
- Cost tracking

### 10. Security Best Practices for AI/ML

#### Model Security

##### Model Protection
- Encrypt model artifacts
- Access control for models
- Version control and tracking
- Secure model endpoints

##### Adversarial Attacks
- **Model Stealing:** Protect model access
- **Data Poisoning:** Validate training data
- **Adversarial Examples:** Input validation
- **Model Inversion:** Limit output information

#### Data Security Best Practices

##### Training Data
- Encrypt at rest and in transit
- Access logging and auditing
- Data minimization
- Sanitize sensitive information

##### Inference Data
- Input validation
- Output filtering
- PII detection and redaction
- Rate limiting

#### Operational Security

##### Least Privilege
- Minimal necessary permissions
- Time-limited access
- Separate production and development
- Regular permission reviews

##### Security Automation
- Automated compliance checks
- Security scanning (IAM Access Analyzer)
- Automated remediation
- Threat detection (GuardDuty)

##### Incident Response
- Incident response plan
- Automated alerting
- Forensic capabilities
- Regular testing and updates

## Study Tips

1. Understand the shared responsibility model for AI/ML
2. Know IAM best practices (least privilege, roles over users)
3. Understand encryption options (KMS, at rest, in transit)
4. Know key regulations (GDPR, CCPA, HIPAA)
5. Understand AWS Artifact for compliance reports
6. Know CloudTrail, CloudWatch, and Config for monitoring
7. Understand VPC security for SageMaker
8. Know data governance and lineage concepts
9. Understand SageMaker Model Monitor capabilities

## Practice Questions

1. What is the AWS shared responsibility model?
   - Answer: AWS is responsible for security OF the cloud (infrastructure), customers are responsible for security IN the cloud (data, applications, access)

2. Which service provides access to compliance reports and certifications?
   - Answer: AWS Artifact

3. How can you ensure AI/ML training data is encrypted at rest?
   - Answer: Use AWS KMS to encrypt S3 buckets and EBS volumes, configure SageMaker to use encryption

4. What is the purpose of CloudTrail in AI/ML governance?
   - Answer: To log API calls for audit trails, compliance, and security analysis

## Key Takeaways

- Shared responsibility model defines AWS and customer security roles
- IAM follows least privilege and use roles over long-term credentials
- Encryption is required at rest (KMS) and in transit (TLS)
- Multiple compliance programs available (HIPAA, PCI DSS, GDPR)
- AWS Artifact provides access to compliance reports
- CloudTrail and CloudWatch are essential for auditing and monitoring
- Data governance includes lifecycle, lineage, and quality management
- VPC endpoints provide private connectivity to AWS services
- SageMaker Model Monitor tracks model performance and drift
- Config and Control Tower enforce governance policies
