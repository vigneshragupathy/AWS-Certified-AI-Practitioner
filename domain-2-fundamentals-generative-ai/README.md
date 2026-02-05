# Domain 2: Fundamentals of Generative AI (24%)

## Overview
This domain covers the core concepts of generative AI, including foundation models, embeddings, and AWS services that enable generative AI applications.

## Topics Covered

### 1. What is Generative AI?

#### Definition
- **Generative AI:** AI systems that can create new content (text, images, audio, code) based on patterns learned from training data
- **Key Difference:** Traditional ML predicts/classifies, Generative AI creates

#### Types of Generative Models
- **Large Language Models (LLMs):** Generate and understand text
- **Diffusion Models:** Generate images from text descriptions
- **Multimodal Models:** Work with multiple types of data (text, images, audio)

### 2. Foundation Models

#### What are Foundation Models?
- **Definition:** Large AI models trained on vast amounts of data that can be adapted for various tasks
- **Characteristics:**
  - Pre-trained on broad data
  - Can be fine-tuned for specific tasks
  - Transfer learning capabilities
  - Few-shot or zero-shot learning

#### Popular Foundation Models
- **GPT (Generative Pre-trained Transformer):** Text generation
- **BERT (Bidirectional Encoder Representations):** Text understanding
- **Claude:** Anthropic's conversational AI
- **Stable Diffusion:** Image generation
- **DALL-E:** Text-to-image generation

### 3. Vectors and Embeddings

#### Embeddings
- **Definition:** Numerical representations of data (text, images) in a multi-dimensional space
- **Purpose:** Enable machines to understand semantic meaning and relationships
- **Example:** Words with similar meanings are close together in embedding space

#### Vector Databases
- **Purpose:** Store and search embeddings efficiently
- **Use Cases:**
  - Semantic search
  - Recommendation systems
  - Similarity matching
- **AWS Service:** Amazon OpenSearch Service with vector engine

#### Vector Operations
- **Similarity Search:** Finding similar items based on vector distance
- **Cosine Similarity:** Measure of similarity between vectors
- **Euclidean Distance:** Straight-line distance between vectors

### 4. Tokenization

#### What is Tokenization?
- **Definition:** Breaking text into smaller units (tokens) for processing
- **Token Types:**
  - Word-level tokens
  - Subword tokens (common in modern LLMs)
  - Character-level tokens

#### Importance in LLMs
- Tokens are the basic units LLMs process
- Token limits affect context window size
- Cost is often calculated per token

### 5. Large Language Models (LLMs)

#### How LLMs Work
- Trained on massive text datasets
- Use transformer architecture
- Predict next token based on context
- Learn patterns, grammar, and knowledge

#### Capabilities
- Text generation and completion
- Summarization
- Translation
- Question answering
- Code generation
- Reasoning and analysis

#### Limitations
- **Hallucinations:** Generating false or nonsensical information
- **Knowledge Cutoff:** Limited to training data timeframe
- **Context Window:** Limited input size
- **Bias:** Reflecting biases in training data
- **No Real Understanding:** Pattern matching, not true comprehension

### 6. Diffusion Models

#### How Diffusion Models Work
- Start with random noise
- Gradually remove noise to create images
- Guided by text prompts or other conditions

#### Use Cases
- Text-to-image generation
- Image editing and inpainting
- Image-to-image translation
- Super-resolution

#### Popular Models
- Stable Diffusion
- DALL-E
- Midjourney

### 7. Multimodal Models

#### Definition
- **Multimodal Models:** AI models that can understand and generate multiple types of data
- **Examples:**
  - Text + Images
  - Text + Audio
  - Text + Video

#### Capabilities
- Image captioning
- Visual question answering
- Text-to-image generation
- Audio-visual understanding

### 8. Prompts and Prompt Engineering

#### What is a Prompt?
- **Definition:** Input text that guides the AI model's output
- **Components:**
  - Instruction: What you want the model to do
  - Context: Background information
  - Input data: Specific data to process
  - Output format: Desired format of response

#### Prompt Engineering Techniques
- **Zero-shot:** No examples provided
- **Few-shot:** Provide a few examples
- **Chain-of-thought:** Ask model to explain reasoning
- **System prompts:** Set model behavior and role
- **Temperature control:** Adjust randomness of outputs

#### Best Practices
- Be clear and specific
- Provide context and examples
- Iterate and refine prompts
- Use delimiters to structure input
- Specify output format

### 9. AWS Services for Generative AI

#### Amazon Bedrock
- **Description:** Fully managed service for foundation models
- **Features:**
  - Access to multiple foundation models (Anthropic, AI21, Cohere, Meta, Stability AI, Amazon)
  - No infrastructure management
  - Private and secure
  - Customization with fine-tuning
  - Retrieval Augmented Generation (RAG)
- **Use Cases:**
  - Chatbots
  - Content generation
  - Document summarization
  - Code generation

#### Amazon SageMaker
- **JumpStart:** Pre-trained foundation models
- **Custom Model Training:** Train your own models
- **Model Deployment:** Deploy at scale
- **Features:**
  - Fine-tuning capabilities
  - Model monitoring
  - Cost optimization

#### Amazon Q
- **Description:** AI-powered assistant for business
- **Capabilities:**
  - Answer questions using company data
  - Generate content
  - Summarize information
  - Code assistance (Amazon Q Developer)

### 10. Retrieval Augmented Generation (RAG)

#### What is RAG?
- **Definition:** Combining information retrieval with text generation
- **How it works:**
  1. Retrieve relevant information from knowledge base
  2. Augment the prompt with retrieved information
  3. Generate response using enhanced context

#### Benefits
- Reduces hallucinations
- Incorporates up-to-date information
- Grounds responses in factual data
- No need to retrain the model

#### Components
- Vector database for embeddings
- Retrieval mechanism
- Foundation model for generation

### 11. Fine-tuning vs. Prompting

#### Prompting
- **Pros:** Quick, no training required, flexible
- **Cons:** Limited control, may not work for complex tasks
- **When to use:** Quick prototypes, simple tasks, testing ideas

#### Fine-tuning
- **Pros:** Better performance, task-specific, consistent style
- **Cons:** Requires training data, time, and resources
- **When to use:** Specific domain knowledge, consistent behavior, production applications

### 12. Business Value of Generative AI

#### Use Cases
- **Customer Service:** AI chatbots and virtual assistants
- **Content Creation:** Marketing copy, articles, social media
- **Code Generation:** Accelerate software development
- **Document Processing:** Summarization, extraction, analysis
- **Creative Design:** Image generation, design variations
- **Personalization:** Customized content and recommendations

#### Benefits
- Increased productivity
- Cost reduction
- Faster time-to-market
- Enhanced creativity
- Improved customer experience
- Scalability

#### Considerations
- Accuracy and reliability
- Cost management (tokens, compute)
- Data privacy and security
- Ethical implications
- Human oversight requirements

## Study Tips

1. Understand the difference between traditional ML and generative AI
2. Know what embeddings and vectors are used for
3. Understand how to use Amazon Bedrock vs. SageMaker
4. Learn prompt engineering best practices
5. Understand RAG and when to use it vs. fine-tuning
6. Know the capabilities and limitations of LLMs
7. Understand multimodal models and their use cases

## Practice Questions

1. What is the purpose of embeddings in generative AI?
   - Answer: To represent data as numerical vectors that capture semantic meaning

2. Which AWS service provides managed access to multiple foundation models?
   - Answer: Amazon Bedrock

3. What is RAG and what problem does it solve?
   - Answer: Retrieval Augmented Generation combines information retrieval with generation to reduce hallucinations and provide up-to-date information

## Key Takeaways

- Generative AI creates new content based on learned patterns
- Foundation models are large, pre-trained models adaptable to various tasks
- Embeddings represent data as vectors to capture semantic meaning
- LLMs have powerful capabilities but also important limitations
- Amazon Bedrock provides managed access to foundation models
- Prompt engineering is crucial for getting good results
- RAG combines retrieval with generation for better accuracy
- Understanding business value and use cases is important for the exam
