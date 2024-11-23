# aws_bedrock_kendra_rag_demo

# **Retrieval Augmented Generation (RAG) using Amazon Bedrock and Amazon Kendra with LangChain**

In today's fast-paced business environment, managing contracts, policies, and compliance documents has become increasingly challenging. AI solutions provided by AWS empower businesses to locate their documents and content instantly using natural language queries, helping businesses to save valuable time.

Brief explainnation of AWS Bedrock and AWS Kendra:

Amazon Bedrock allows businesses to build and scale generative AI applications by using **foundation models (FMs)** without needing to manage the underlying infrastructure. Bedrock provides access to multiple pre-trained foundation models from different providers, enabling users to choose the model that best suits their use case. Among the models available on Amazon Bedrock is **Claude**, developed by Anthropic. Claude is designed to be helpful, ethical, and safe, making it ideal for a wide range of generative AI use cases. **Claude 3.0 Haiku** will be use as an example in this code.

Amazon Kendra is an intelligent enterprise search service provided by AWS that enables users to search for and retrieve relevant information from structured and unstructured data across various data sources. It uses **machine learning (ML)** and **natural language processing (NLP)** to understand the intent behind a user’s query and provide accurate, contextually relevant results, even when the query is phrased in natural language.

This is a simple architecture for this code:

![image-2.png](attachment:image-2.png)

Processes:
1. Document Upload: Users upload documents (e.g., PDFs, Word files, images, etc.) to Amazon Simple Storage Service (S3).

2. Indexing: Uploaded documents in Amazon S3 are processed and indexed by Amazon Kendra.

3. Query: User submits a query to the system through an application (e.g., chatbot, search interface).

4. Retrieval: Amazon Kendra searches the indexed documents to find the most relevant content for the user’s query.

5. Response: Retrieved information is passed back to Amazon Bedrock, which processes it and generates a clear, human-like response.

The code in this repo demonstrates how AWS Bedrock and Kendra can assist in quickly searching through a large volume of documents within seconds.
