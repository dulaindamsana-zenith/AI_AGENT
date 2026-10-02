# Quantum Cyber Physicist AI Chatbot

A Python-based command-line chatbot interface utilizing the **Gemini 2.5 Flash** model via the official `google-genai` SDK. This agent is hard-coded to exclusively assist users on their journey toward becoming a **Quantum Cyber Physicist**.

## Features
- **Strict Domain Locking**: The agent automatically rejects non-relevant prompts with a standardized refusal message.
- **Google Search Integration**: Grounded responses utilizing Gemini's integrated Google Search tool.
- **Session History Logging**: Automatically appends interaction logs locally to a `chat.history` text file.
- **Formatted Terminal Output**: Uses ANSI escape colors to separate user prompts from agent responses clearly.

## Prerequisites
- Python 3.10 or higher
- A Gemini API Key from Google AI Studio

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY
   ```

2. **Install Dependencies**
   ```bash
   pip install google-genai python-dotenv
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory and add your API key:
   ```env
   GEMINI_API_KEY=your_actual_api_key_here
   ```

## Usage
Run the script to launch the interactive terminal session:
```bash
python main.py
```
Type `exit` or `quit` to end the session.

## Customization
You can easily change the behavior, scope, and personality of this chatbot by modifying the `system_instruction` parameter inside `main.py`.

Locate this block in the source code:
```python
config=types.GenerateContentConfig(
    system_instruction="""Your custom prompt goes here...""",
    # ...
)
```
Replace the text inside the triple quotes with any topic restrictions, guiding philosophies, or operating protocols that fit your needs.

## License
This project is licensed under MPL-2.0
