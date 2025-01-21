Sure! Here's an updated version of the README with the name **VidAnalyze**:

---

# VidAnalyze

**VidAnalyze** is an AI-powered web application that allows users to upload videos, process them, and receive intelligent summaries or answers based on video content. Built with FastAPI, this app leverages Google’s Gemini AI model and other advanced tools to analyze and summarize video content quickly and efficiently.

## Features

- **Video Upload**: Upload videos in MP4 format for processing.
- **Video Analysis**: Submit queries related to the video, and get AI-generated insights or summaries.
- **Background Processing**: Video analysis is handled in the background to ensure smooth user experience.
- **AI-Powered Summarization**: Uses advanced AI models to analyze and provide relevant summaries based on user queries.

## Requirements

- Python 3.8+
- FastAPI
- Uvicorn
- google-generativeai
- Phi AI library
- DuckDuckGo API
- Python-dotenv

### Install Dependencies

To get started, clone the repository and install the necessary dependencies using `pip`:

```bash
git clone https://github.com/yourusername/vidanalyze.git
cd vidanalyze
pip install -r requirements.txt
```

### Environment Variables

Before running the application, you need to set up the required environment variables. Create a `.env` file in the root directory of the project and include the following:

```bash
GOOGLE_API_KEY=your_google_api_key_here
```

You can obtain your `GOOGLE_API_KEY` by creating a project in the [Google Cloud Console](https://console.cloud.google.com/) and enabling the relevant API.

## Running the Application

To run the FastAPI application locally, execute the following command:

```bash
uvicorn main:app --reload
```

This will start the server at `http://127.0.0.1:8000`.

### Endpoints

1. **Home Page**:  
   URL: `GET /`  
   Displays the homepage with a form to upload videos.

2. **Upload Video**:  
   URL: `POST /upload`  
   Allows users to upload a video for processing. This is a background task, and once the video is uploaded, users will receive a `task_id` that can be used to track the progress and results.

   **Request Example**:
   ```bash
   POST /upload
   Content-Type: multipart/form-data
   File: video.mp4
   ```

3. **Analyze Video**:  
   URL: `POST /analyze/{task_id}`  
   After uploading a video, users can submit a query to get insights or summaries related to the video content using the `task_id`.

   **Request Example**:
   ```bash
   POST /analyze/{task_id}
   query=What are the main points in this video?
   ```

   **Response Example**:
   ```json
   {
     "success": true,
     "analysis": {
       "id": "unique-analysis-id",
       "query": "What are the main points in this video?",
       "result": "This video discusses the following key points: ...",
       "timestamp": "2025-01-21T12:34:56Z",
       "video_id": "task-id"
     }
   }
   ```


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Let me know if you need further changes or additions!
