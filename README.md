# Phidata Video AI Summarizer Agent 🎥🎤

This application is a **Multimodal AI Agent** designed to analyze video content and provide detailed, actionable insights. Powered by **Gemini 2.0 Flash Exp**, it leverages advanced AI models and tools for video analysis and supplementary web research.

**Live URL:   https://videosummarygenerator.streamlit.app/**
## Features

- **Video Upload**: Upload video files in formats like `.mp4`, `.mov`, or `.avi`.
- **AI-Powered Analysis**: Analyze video content using AI and gather additional context from the web.
- **Interactive Querying**: Ask specific questions or request insights about the video content.
- **User-Friendly Interface**: Built with Streamlit for an intuitive and responsive UI.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the environment variables:
   - Create a `.env` file in the root directory.
   - Add the following keys (replace with your actual API keys):
     ```env
     PHI_API_KEY=your-phi-api-key
     GOOGLE_API_KEY=your-google-api-key
     GROQ_API_KEY=your-groq-api-key
     ```

## Usage

1. Run the application:
   ```bash
   streamlit run app.py
   ```

2. Open the application in your browser (usually at `http://localhost:8501`).

3. Upload a video file, enter your query, and click **Analyze Video** to get insights.

## Dependencies

The application requires the following Python packages (see [requirements.txt](requirements.txt) for the full list):
- `streamlit`: For building the user interface.
- `google-generativeai`: For AI-powered video analysis.
- `duckduckgo-search`: For supplementary web research.
- `python-dotenv`: For managing environment variables.
- And more...

## File Structure

```
.
├── 

app.py

              # Main application file
├── 

requirements.txt

    # List of dependencies
├── .env                # Environment variables (ignored by Git)
├── .gitignore          # Git ignore file
```

## Key Components

- **Agent Initialization**: The AI agent is initialized using the `initialize_agent` function in `app.py`.
- **Video Upload and Processing**: Users can upload video files, which are temporarily stored and processed.
- **AI Analysis**: The AI agent analyzes the video and responds to user queries with detailed insights.

## Environment Variables

The application uses the following

 environment

 variables:
- `PHI_API_KEY`: API key for Phi tools.
- `GOOGLE_API_KEY`: API key for Google Generative AI.
- `GROQ_API_KEY`: API key for Groq.

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests to improve the application.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- **Phidata**: For providing the AI tools and models.
- **Streamlit**: For the interactive UI framework.
- **DuckDuckGo**: For web search integration.
- **Google Generative AI**: For video analysis capabilities.
```

