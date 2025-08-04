ShayarAI 📜
A poetic personality chatbot that transforms everyday language into beautiful, lyrical verses using the power of Google's Gemini LLM.

This project turns any simple message into a thoughtful, rhyming poem, creating an immersive experience as if you're conversing with a digital poet.

✨ Features
AI-Powered Poetry: Converts any user input into a unique, context-aware poem in real-time.

Crafted Persona: Utilizes detailed prompt engineering to give ShayarAI a consistent, thoughtful, and lyrical personality.

Immersive Experience: Features a typing animation that simulates a poet composing verses live for the user.

Robust & Tested: Designed to handle a wide range of emotional inputs, questions, and edge cases gracefully.

🚀 Demo
Here is a brief demonstration of ShayarAI in action.



🛠️ Tech Stack
Language: Python

LLM: Google Gemini API (Gemini 1.5 Flash/Pro)

Core Library: google-generativeai

Environment: Google Colab / Jupyter Notebook

⚙️ Getting Started
To get a local copy up and running, follow these simple steps.

Prerequisites
You will need a Google Gemini API Key to run this project.

Get your API key from Google AI Studio.

Installation
Clone the repository:

Bash

git clone https://github.com/your-username/ShayarAI.git
Navigate to the project directory:

Bash

cd ShayarAI
Install dependencies:
If you're using the .ipynb notebook in Google Colab, the installation command is included at the top of the notebook. For a local setup, you can install the required package directly:

Bash

pip install google-generativeai
Set up your API Key:
It is highly recommended to set your API key as an environment variable rather than hardcoding it.

In Google Colab: Use the "Secrets" (🔑) tab to store your key with the name GEMINI_API_KEY.

For local development:

Bash

export GEMINI_API_KEY='your_api_key_here'
Run the Chatbot:
Open the ShayarAI.ipynb notebook and run the cells in order. The final cell containing the chat() function will start the interactive session.

🧠 The Core: Prompt Engineering
The soul of ShayarAI lies not just in the model, but in the system prompt. The bot's ability to maintain its persona, adhere to a rhyming scheme, and reflect user emotions is a direct result of carefully engineered instructions. This prompt defines the rules, constraints, and creative spirit, guiding the LLM to act as a thoughtful poet rather than a generic text generator.

🤝 Acknowledgments
Thanks to Google for providing the powerful and accessible Gemini API.

Inspired by the creative potential at the intersection of art and artificial intelligence.
