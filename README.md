# Video AI Summarizer Agent 🎥🎤🖬

## Overview
The **Video AI Summarizer Agent** is a multimodal AI-powered application designed to analyze video content and provide actionable insights. Leveraging Google's Gemini 2.0 Flash Exp model and DuckDuckGo for web research, this tool allows users to upload video files, ask specific questions, and receive concise, user-friendly summaries and insights.

This project is built using **Streamlit** for the frontend interface and integrates advanced AI capabilities to process and analyze video content dynamically.

---

## Features
- **Video Analysis**: Upload video files (MP4, MOV, AVI) for AI-driven content analysis.
- **Multimodal AI**: Utilizes Google's Gemini 2.0 Flash Exp model for video and text processing.
- **Web Research Integration**: Incorporates DuckDuckGo to gather additional context and insights.
- **User-Friendly Interface**: Simple and intuitive interface powered by Streamlit.
- **Customizable Queries**: Users can ask specific questions or request insights about the video content.

---

## Technologies Used
- **Streamlit**: For building the web application interface.
- **Google Gemini 2.0 Flash Exp**: For video and text analysis.
- **DuckDuckGo API**: For supplementary web research.
- **Google Generative AI SDK**: For video file processing and analysis.
- **Python**: Primary programming language for backend logic.
- **Environment Management**: `dotenv` for managing environment variables.

---

## How It Works
1. **Upload a Video**: Users upload a video file (MP4, MOV, or AVI) through the Streamlit interface.
2. **Ask a Question**: Users provide a specific query or insight they want from the video.
3. **AI Processing**: The video is processed using Google's Gemini model, and additional context is gathered via DuckDuckGo.
4. **Get Insights**: The AI agent generates a concise, actionable response based on the video content and user query.

---

## Installation and Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/video-ai-summarizer.git
   cd video-ai-summarizer
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**:
   - Create a `.env` file in the root directory.
   - Add your Google API key:
     ```plaintext
     GOOGLE_API_KEY=your_api_key_here
     ```

4. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

5. **Access the Application**:
   - Open your browser and navigate to `http://localhost:8501`.

---

## Usage
1. Upload a video file using the file uploader.
2. Enter your query or insight request in the text area.
3. Click the **"Analyze Video"** button to process the video and generate insights.
4. View the analysis results displayed on the screen.

---

## Example Queries
- "What is the main topic of this video?"
- "Summarize the key points discussed in the video."
- "Identify any notable events or actions in the video."
- "Provide additional context about the people or places mentioned in the video."

---

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push to the branch.
4. Submit a pull request with a detailed description of your changes.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **Google Gemini**: For providing the advanced AI model for video and text analysis.
- **Streamlit**: For enabling the creation of a user-friendly web interface.
- **DuckDuckGo**: For supporting web research capabilities.

---

## Contact
For questions or feedback, please reach out to:
- **Your Name**: [Your Email Address](mailto:your.email@example.com)
- **GitHub**: [Your GitHub Profile](https://github.com/your-username)

---

Enjoy using the **Video AI Summarizer Agent**! 🎥🤖
