# AWS Services Quick Reference

## Core AI/ML Services

### Amazon Bedrock
- **Purpose:** Managed access to foundation models
- **Models Available:**
  - Anthropic Claude
  - AI21 Jurassic
  - Cohere
  - Meta Llama
  - Stability AI
  - Amazon Titan
- **Key Features:**
  - No infrastructure management
  - Private and secure
  - Fine-tuning support
  - RAG capabilities
  - Model evaluation
- **Use Cases:**
  - Chatbots and virtual assistants
  - Content generation
  - Document summarization
  - Code generation

### Amazon SageMaker
- **Purpose:** Complete ML platform for building, training, and deploying models
- **Components:**
  - **Studio:** Integrated development environment
  - **Notebooks:** Jupyter notebooks
  - **Training:** Distributed training
  - **Inference:** Real-time and batch
  - **JumpStart:** Pre-trained models
  - **Autopilot:** Automated ML
  - **Canvas:** No-code ML
- **Additional Features:**
  - Model Monitor: Track model quality
  - Clarify: Bias detection and explainability
  - Data Wrangler: Data preparation
  - Feature Store: Centralized feature repository
  - Pipelines: MLOps workflows
- **Use Cases:**
  - Custom ML model development
  - Model training and fine-tuning
  - Production model deployment
  - ML experimentation

### Amazon Q
- **Purpose:** AI-powered assistant for business and development
- **Variants:**
  - **Amazon Q Business:** Enterprise AI assistant
  - **Amazon Q Developer:** Code assistance and development
- **Key Features:**
  - Query company data
  - Generate content
  - Summarize information
  - Code generation and debugging
- **Use Cases:**
  - Internal knowledge base Q&A
  - Developer productivity
  - Business intelligence

## NLP Services

### Amazon Comprehend
- **Purpose:** Natural language processing
- **Features:**
  - Sentiment analysis
  - Entity recognition
  - Key phrase extraction
  - Language detection
  - Topic modeling
  - PII detection
- **Use Cases:**
  - Customer feedback analysis
  - Document classification
  - Social media monitoring

### Amazon Translate
- **Purpose:** Neural machine translation
- **Features:**
  - Real-time translation
  - Batch translation
  - Custom terminology
  - 75+ languages
- **Use Cases:**
  - Website localization
  - Content translation
  - Customer support

### Amazon Transcribe
- **Purpose:** Speech-to-text
- **Features:**
  - Real-time transcription
  - Batch transcription
  - Speaker identification
  - Custom vocabulary
  - PII redaction
- **Use Cases:**
  - Call center analytics
  - Meeting transcription
  - Subtitles and captions

### Amazon Polly
- **Purpose:** Text-to-speech
- **Features:**
  - Neural TTS
  - Multiple voices and languages
  - SSML support
  - Speech marks
- **Use Cases:**
  - Accessibility features
  - Voice assistants
  - Content narration

### Amazon Lex
- **Purpose:** Build conversational interfaces
- **Features:**
  - Natural language understanding
  - Automatic speech recognition
  - Dialog management
  - Integration with Lambda
- **Use Cases:**
  - Chatbots
  - Voice assistants
  - Customer service automation

## Computer Vision Services

### Amazon Rekognition
- **Purpose:** Image and video analysis
- **Features:**
  - Object and scene detection
  - Facial analysis
  - Face comparison
  - Text in images (OCR)
  - Content moderation
  - Celebrity recognition
  - Custom labels
- **Use Cases:**
  - Content moderation
  - Security and surveillance
  - Media analysis

### Amazon Textract
- **Purpose:** Extract text and data from documents
- **Features:**
  - OCR
  - Form extraction
  - Table extraction
  - Document structure analysis
- **Use Cases:**
  - Document processing
  - Invoice processing
  - Identity verification

## Specialized AI Services

### Amazon Personalize
- **Purpose:** Personalized recommendations
- **Features:**
  - Real-time recommendations
  - Batch recommendations
  - Similar items
  - User segmentation
- **Use Cases:**
  - Product recommendations
  - Content recommendations
  - Marketing personalization

### Amazon Forecast
- **Purpose:** Time-series forecasting
- **Features:**
  - Automated ML for forecasting
  - Multiple algorithms
  - What-if analysis
- **Use Cases:**
  - Demand forecasting
  - Resource planning
  - Financial forecasting

### Amazon Fraud Detector
- **Purpose:** Fraud detection
- **Features:**
  - Pre-built fraud models
  - Custom models
  - Real-time fraud detection
- **Use Cases:**
  - Payment fraud detection
  - Account takeover prevention
  - Online identity fraud

### Amazon CodeWhisperer
- **Purpose:** AI-powered code suggestions
- **Features:**
  - Code completion
  - Security scanning
  - Reference tracking
  - Multiple languages
- **Use Cases:**
  - Developer productivity
  - Code quality improvement
  - Learning new APIs

### AWS DeepRacer
- **Purpose:** Reinforcement learning education
- **Features:**
  - Autonomous racing
  - RL training
  - Competitions
- **Use Cases:**
  - Learning RL concepts
  - Team building
  - Education

## Supporting Services

### Amazon OpenSearch Service
- **Purpose:** Search and analytics
- **Features:**
  - Vector search (k-NN)
  - Text search
  - Log analytics
  - Visualization
- **Use Cases:**
  - Semantic search
  - RAG applications
  - Log analysis

### AWS Glue
- **Purpose:** ETL and data catalog
- **Features:**
  - Data catalog
  - ETL jobs
  - Data quality
  - Data lineage
- **Use Cases:**
  - Data preparation
  - Data governance
  - ML data pipelines

### Amazon S3
- **Purpose:** Object storage
- **Features:**
  - Unlimited storage
  - Versioning
  - Encryption
  - Lifecycle policies
- **Use Cases:**
  - Training data storage
  - Model artifact storage
  - Data lakes

### AWS Lambda
- **Purpose:** Serverless compute
- **Features:**
  - Event-driven execution
  - Auto-scaling
  - Pay per use
- **Use Cases:**
  - Inference endpoints
  - Data processing
  - Workflow automation

### Amazon DynamoDB
- **Purpose:** NoSQL database
- **Features:**
  - Millisecond latency
  - Auto-scaling
  - Serverless
- **Use Cases:**
  - Feature storage
  - Session data
  - Metadata storage

## Security and Governance

### AWS IAM
- **Purpose:** Identity and access management
- **Key Concepts:**
  - Users, groups, roles
  - Policies
  - MFA
  - Service control policies

### AWS KMS
- **Purpose:** Key management
- **Features:**
  - Encryption key creation
  - Key rotation
  - Access policies
  - Audit logging

### AWS CloudTrail
- **Purpose:** API logging
- **Features:**
  - API call tracking
  - Compliance auditing
  - Security analysis
  - Multi-region trails

### Amazon CloudWatch
- **Purpose:** Monitoring and observability
- **Features:**
  - Metrics
  - Logs
  - Alarms
  - Dashboards

### AWS Config
- **Purpose:** Resource compliance
- **Features:**
  - Configuration tracking
  - Compliance rules
  - Remediation
  - Conformance packs

### AWS Artifact
- **Purpose:** Compliance reports
- **Features:**
  - SOC reports
  - PCI reports
  - ISO certifications
  - BAA downloads

### Amazon Macie
- **Purpose:** Data security and privacy
- **Features:**
  - Sensitive data discovery
  - Data classification
  - Security alerts
- **Use Cases:**
  - PII detection
  - Data security audits
  - Compliance monitoring

## Pricing Models

### On-Demand Pricing
- **Bedrock:** Per token (input/output)
- **SageMaker:** Per instance hour
- **AI Services:** Per API call or unit processed

### Provisioned Throughput
- **Bedrock:** Reserved model capacity
- **SageMaker:** Reserved instances

### Free Tier
- Many services offer free tier
- Limited usage per month
- Great for learning and testing

## Service Selection Guide

### For Text Generation
- **Simple:** Amazon Bedrock
- **Custom:** SageMaker with foundation models

### For NLP Tasks
- **Pre-built:** Amazon Comprehend
- **Custom:** SageMaker

### For Computer Vision
- **Pre-built:** Amazon Rekognition
- **Custom:** SageMaker

### For Speech
- **Speech-to-text:** Amazon Transcribe
- **Text-to-speech:** Amazon Polly

### For Chatbots
- **Conversational interface:** Amazon Lex + Bedrock
- **Custom:** SageMaker

### For Recommendations
- **Ready-made:** Amazon Personalize
- **Custom:** SageMaker

## Common Integration Patterns

### Data Pipeline
S3 → Glue → SageMaker → S3 → Application

### Inference Pipeline
Application → API Gateway → Lambda → Bedrock/SageMaker → Application

### RAG Architecture
User Query → Embeddings → OpenSearch (vector search) → Context + Query → Bedrock → Response

### Monitoring
SageMaker/Bedrock → CloudWatch Metrics → CloudWatch Alarms → SNS

### Compliance
All Services → CloudTrail → S3 → Athena (analysis) → QuickSight (visualization)
