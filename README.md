#Twin AI

Twin AI is a full-stack, cloud-ready AI application designed to act as a personal "Digital Twin." Powered by an LLM backend (integrating AWS Bedrock / Nova-lite), this agent engages with visitors by faithfully representing professional context, work history, and communication styles.

Key Features:

Intelligent Conversational Agent: Leverages AWS Bedrock to process natural language alongside a persistent historical memory window (last 50 exchanges).
Context-Aware: Dynamically reads and extracts personal facts, stylistic guides, and PDF resumes using pypdf to ground the AI's identity.
Cloud-Ready Architecture: Includes a deploy.py script that neatly packages the FastAPI application via mangum to be securely run on AWS Lambda.
Persistent Memory: Uses local file-based storage or AWS S3 buckets to track user chat session contexts over time.
Responsive Frontend UI: A sleek Next.js React frontend built with Tailwind CSS v4 to provide a modern, low-latency chat interface.
Tech Stack:

Frontend: Next.js (React), Tailwind CSS.
Backend: Python 3.12, FastAPI, Uvicorn.
AI & Cloud infra: AWS Bedrock, Amazon S3, AWS Lambda, boto3.
