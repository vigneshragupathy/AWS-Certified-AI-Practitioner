# Domain 1: Fundamentals of AI and ML (20%)

## Overview
This domain covers the foundational concepts of Artificial Intelligence and Machine Learning, including core terminology, learning types, and key concepts.

## Topics Covered

### 1. Core AI and ML Terminology

#### Artificial Intelligence (AI)
- **Definition:** The simulation of human intelligence in machines programmed to think and learn
- **Types:**
  - Narrow AI (Weak AI): Designed for specific tasks
  - General AI (Strong AI): Theoretical AI with human-like intelligence
  
#### Machine Learning (ML)
- **Definition:** A subset of AI that enables systems to learn and improve from experience without explicit programming
- **Key Concepts:**
  - Training: Process of teaching a model using data
  - Features: Input variables used to make predictions
  - Labels: Target variable or output in supervised learning
  - Model: Mathematical representation learned from data

### 2. Types of Machine Learning

#### Supervised Learning
- **Definition:** Learning from labeled data
- **Use Cases:**
  - Classification: Categorizing data into predefined classes
  - Regression: Predicting continuous values
- **Examples:**
  - Email spam detection
  - House price prediction
  - Image classification

#### Unsupervised Learning
- **Definition:** Learning from unlabeled data to find patterns
- **Use Cases:**
  - Clustering: Grouping similar data points
  - Dimensionality reduction: Simplifying data while preserving information
- **Examples:**
  - Customer segmentation
  - Anomaly detection
  - Market basket analysis

#### Reinforcement Learning
- **Definition:** Learning through trial and error with rewards/penalties
- **Use Cases:**
  - Game playing
  - Robotics
  - Autonomous vehicles

### 3. Natural Language Processing (NLP)

#### Key Concepts
- **Text Processing:** Converting text into a format machines can understand
- **Tokenization:** Breaking text into words or subwords
- **Named Entity Recognition (NER):** Identifying entities like names, dates, locations
- **Sentiment Analysis:** Determining emotional tone of text

#### Common NLP Tasks
- Machine translation
- Text summarization
- Question answering
- Chatbots and conversational AI

### 4. Deep Learning

#### Neural Networks
- **Definition:** Computing systems inspired by biological neural networks
- **Components:**
  - Neurons: Basic processing units
  - Layers: Input, hidden, and output layers
  - Weights and biases: Parameters learned during training
  - Activation functions: Non-linear transformations

#### Types of Neural Networks
- **Convolutional Neural Networks (CNN):** For image processing
- **Recurrent Neural Networks (RNN):** For sequential data
- **Transformers:** Modern architecture for NLP and beyond

### 5. Key ML Concepts

#### Model Training
- **Training Set:** Data used to train the model
- **Validation Set:** Data used to tune hyperparameters
- **Test Set:** Data used to evaluate final model performance

#### Model Evaluation
- **Accuracy:** Percentage of correct predictions
- **Precision:** True positives / (True positives + False positives)
- **Recall:** True positives / (True positives + False negatives)
- **F1 Score:** Harmonic mean of precision and recall

#### Overfitting and Underfitting
- **Overfitting:** Model performs well on training data but poorly on new data
- **Underfitting:** Model performs poorly on both training and test data
- **Solutions:** 
  - Regularization
  - Cross-validation
  - More training data
  - Feature selection

### 6. Bias and Fairness

#### Types of Bias
- **Data Bias:** Bias present in training data
- **Algorithm Bias:** Bias introduced by the algorithm itself
- **Human Bias:** Bias from human decisions in the ML pipeline

#### Fairness Considerations
- Equal opportunity
- Demographic parity
- Individual fairness
- Group fairness

### 7. Inferencing

#### Definition
- **Inference:** Using a trained model to make predictions on new data

#### Types
- **Batch Inference:** Processing multiple inputs at once
- **Real-time Inference:** Processing inputs as they arrive
- **Edge Inference:** Running models on edge devices

## When to Use AI/ML

### Good Use Cases
- Pattern recognition in large datasets
- Repetitive decision-making tasks
- Personalization and recommendations
- Predictive analytics
- Computer vision tasks
- Natural language understanding

### Not Suitable For
- Tasks requiring human empathy
- Situations with insufficient data
- High-stakes decisions without human oversight
- Problems better solved with traditional programming

## AWS Services for AI/ML Fundamentals

- **Amazon SageMaker:** Complete ML platform
- **Amazon Comprehend:** NLP service
- **Amazon Rekognition:** Computer vision service
- **Amazon Translate:** Neural machine translation
- **Amazon Transcribe:** Speech-to-text
- **Amazon Polly:** Text-to-speech

## Study Tips

1. Understand the difference between AI, ML, and Deep Learning
2. Know when to use supervised vs unsupervised learning
3. Understand model evaluation metrics
4. Recognize common bias and fairness issues
5. Know the basics of NLP and computer vision
6. Understand the ML pipeline from data to deployment

## Practice Questions

1. What type of learning is used when you want to categorize emails as spam or not spam?
   - Answer: Supervised learning (classification)

2. What is the difference between overfitting and underfitting?
   - Answer: Overfitting means the model memorizes training data but performs poorly on new data; underfitting means the model is too simple to capture patterns

3. Which AWS service would you use for sentiment analysis of customer reviews?
   - Answer: Amazon Comprehend

## Key Takeaways

- ML is a subset of AI focused on learning from data
- Different learning types (supervised, unsupervised, reinforcement) suit different problems
- Model evaluation and addressing bias are crucial for successful ML
- Deep learning uses neural networks for complex pattern recognition
- NLP enables machines to understand and generate human language
- Understanding when to use ML is as important as knowing how to use it
