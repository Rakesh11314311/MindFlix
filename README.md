# Retrieval Augmented Generation
Implements a Retriever to retrieve a youtube video and give the information being queried, based on the User Question.

## Features
a. Downloads the video
b. Transcribes the Video using the following approaches:
c. Extract Keyframes/Scenes from the video and generate frame/scene description leveraging open-source Large Vision Language Models (LVLMs).
d. Captures the Video Metadata
e. Chunk the video metadata and Store it in a VectorDB

## Instructions to run the model

1. **Install Dependencies**

Install the required packages using pip. The required packages are given in requirements.txt

4. **Upload PDF:** Once Streamlit server is running, a browser window will open. Upload your PDF file using the provided file uploader.

5. **Add Your Prompt:** Enter your query or prompt related to the content of the uploaded PDF in the chat interface.

6. **Wait for Results:** DocBot will process your prompt, extract relevant information, generate captions for images, and display the most relevant image along with the answer to your query.

## APIs Used
DocBot utilizes the following APIs and models:

- **Gemini Pro Vision:** Used for image captioning, providing descriptive captions for images extracted from the PDF.

- **GPT-3.5-Turbo:** Employs GPT-3.5 for text-based question-answering tasks, extracting relevant information from the PDF.

- **YOLO(from Roboflow):** A custom-trained YOLO V5 model(on a PDF, which was custom trained on bounding boxes) specifically designed for image detection within PDF documents.
