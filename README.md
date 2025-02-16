# SMUPal Chatbot

## Overview
SMUPal is an AI chatbot designed to assist students and the broader community at Saint Mary's University (SMU). The chatbot provides clear, empathetic, and accessible guidance on a variety of university-related topics, including campus resources, academic support, student life, and more.

SMUPal is trained on a curated dataset obtained from the Saint Mary's University website and the Saint Mary's University Students' Association (SMUSA). It utilizes keyword recognition, encouragement-based responses, and resource-based guidance to create an effective, student-friendly AI assistant. The chatbot is powered by IBM Watsonx Orchestrate and is currently hosted on a static website generated with Jekyll for demonstration purposes.

## Features
- **Student-Oriented Design**: Tailored to meet the needs of students, providing both academic and emotional support.
- **SMU-Specific Knowledge**: Trained with customized data relevant to Saint Mary's University.
- **Human Agent Integration**: Allows users to connect with university staff or support services when necessary.
- **Multilingual Support**: Supports multiple languages, including English, Chinese, and Japanese.
- **Watsonx AI Technology**: Powered by IBM Watsonx Orchestrate for accurate and responsive AI interactions.
- **User-Friendly Interface**: Intuitive design with buttons for quick responses and a text input field for custom queries.
- **Emotional Support**: Provides guidance on common student concerns, such as exam stress and mental well-being.

## Current Training Data
SMUPal is currently trained on a limited dataset for demonstration purposes, including:
- SMUSA resources
- "New to SMU" program information
- On-campus job opportunities
- On-campus dining options
- Residence resources
- Comprehensive details on first-year Computer Science courses at SMU
- Basic general question-answering capabilities

## Installation & Deployment
### Prerequisites
- Python 3.8+
- IBM Watsonx Orchestrate API credentials
- Jekyll (for static site deployment)

### Setup Instructions
1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-repository/smupal.git
   cd smupal
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Set up IBM Watsonx API credentials:**
   - Create an `.env` file in the root directory and add your API keys:
     ```sh
     IBM_API_KEY=your_api_key_here
     IBM_SERVICE_URL=your_service_url_here
     ```

4. **Run the chatbot locally:**
   ```sh
   python chatbot.py
   ```

5. **Deploy on Jekyll-based static website:**
   - Ensure Jekyll is installed:
     ```sh
     gem install jekyll bundler
     ```
   - Build the website:
     ```sh
     jekyll build
     ```
   - Serve the website:
     ```sh
     jekyll serve
     ```

## Usage Guide
1. Visit the chatbot webpage.
2. Use the interactive buttons for quick questions or type your query into the chat field.
3. Receive relevant responses or be guided to appropriate resources.
4. If needed, escalate your query to a human agent through the chatbot.

## Future Improvements
- Expanding training data to cover more SMU-related topics.
- Integrating additional AI-powered features for improved contextual understanding.
- Deploying on a permanent server with increased stability and performance.
- Enhancing multilingual support with additional languages.
- Improving chatbot personalization based on user preferences.

## Contributors
- **Abdiaziz Muse**
- **Yilin Huang**
- **Muhammad Shaheer**

## Acknowledgments
SMUPal was developed as part of the IBM Watsonx Education Challenge, where it won second place. Special thanks to IBM and SMU for their support in this initiative.
