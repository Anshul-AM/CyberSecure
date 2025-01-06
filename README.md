# CyberSecure: A Virtual Assistant for Cybersecurity Awareness and Best Practices![Screenshot 2025-01-05 224625](https://github.com/user-attachments/assets/2b1be70d-1c9b-4d18-8b9d-c3b7376167b6)
## Introduction
In today’s digital age, cybersecurity is paramount. Threats such as malicious software, hackers, and viruses pose significant risks to individuals and organizations alike. To address these challenges, **CyberSecure** was developed as a virtual assistant aimed at raising cybersecurity awareness and providing actionable best practices.
### Key Features:
- Tailored to two primary user groups:
  - **Public Users**: Guidance on avoiding scams, protecting personal information, and staying safe online.
  - **Organizational Users**: Support for employees and IT teams in implementing internal security protocols, managing digital assets, and detecting social engineering attacks.
- Built using a **Retrieval-Augmented Generation (RAG)** pipeline for precise, context-driven responses.
- Powered by advanced **Large Language Models (LLMs)**: Gemma, Llama, and Qwen.

---

## Data
### Document Corpus:
The dataset includes documents covering a wide range of cybersecurity topics, such as malware, social engineering, and organizational security policies. Key resources include:  
1. **An Introduction to Malware** by Robin Sharp  
   - Overview of malware types (viruses, worms, trojans) and mitigation strategies.
2. **Cybersecurity Handbook** by ROF Network  
   - Comprehensive guide with tips on device security, encryption, and safe browsing.
3. **Cybersecurity for Small Business: Cybersecurity Basics**  
   - Focuses on phishing attacks, data breaches, and employee training for small businesses.
4. **Basic Cyber Security: A Guide for All to Manage Digital Security**  
   - Practical steps for managing digital safety, including password management and software updates.

### Document Properties:
- **Corpus Size**: Over 34,896 words, supporting at least 30 unique queries.
- **Format**: All documents are provided in PDF format.

---

## System Architecture
The system uses a **RAG pipeline** for processing queries. Below is an overview of the workflow:

1. **User Query**: Input collected via the AI application.
2. **Retrieval**: Relevant information is fetched from the knowledge base using the Chroma retrieval system.
3. **LLM Processing**: The retrieved data is integrated with the query to generate a contextually accurate response.
4. **Response Delivery**: The response is returned to the user through the application.

## LLM Models Used
CyberSecure leverages the following models for context-aware, real-time responses:
- **Gemma-2-2B-IT**
- **Qwen 2.5 1.5 B-Instruct**
- **Llama-3.2-3B-Instruct**

---

## Evaluation Metrics
The performance of the RAG models was evaluated based on:
1. **Accuracy**: User-rated accuracy of responses (scale: 1–5).
2. **Groundedness**: Cosine similarity between model output and source documents.
3. **Speed**: Time taken by the model to generate a response (in seconds).

### Results:
| Model   | Average Accuracy (%) | Average Groundedness (%) | Average Speed (s) |
|---------|-----------------------|--------------------------|-------------------|
| Gemma   | 75.15                | 71.37                   | 11.27            |
| Llama   | 73.75                | 71.30                   | 11.22            |
| Qwen    | **86.67**            | **76.65**               | 12.11            |

### Key Findings:
- **Qwen**: Achieved the highest accuracy (86.67%) and groundedness (76.65%).
- **Gemma**: The fastest model with an average response time of 11.27 seconds.
- **Llama**: Balanced performance but slightly lagged behind Qwen in accuracy and groundedness.

---

## Presentation Video
For a detailed walkthrough of the project, check out the [presentation video](https://drive.google.com/file/d/1E2hXcFCWfdRaGQ3QpPViWl0HyeZtaPo5/view?usp=sharing).

---

## Conclusion
CyberSecure successfully demonstrates the potential of RAG pipelines combined with advanced LLMs in addressing cybersecurity challenges. The virtual assistant is a valuable tool for both individuals and organizations, providing precise, actionable advice to enhance online safety.  
- **Qwen**: Best suited for tasks requiring high accuracy and reliability.  
- **Gemma**: Ideal for scenarios demanding rapid responses.  
- **Llama**: Offers balanced performance across all metrics.  


