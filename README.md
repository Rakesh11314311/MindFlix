# Retrieval Augmented Generation
Implements a Retriever to retrieve a YouTube video and give the information being queried, based on the User Question.

## Features
a. Downloads the video
b. Transcribes the Video using the following approaches:
c. Extract Keyframes/Scenes from the video and generate frame/scene description leveraging open-source Large Vision Language Models (LVLMs).
d. Captures the Video Metadata
e. Chunk the video metadata and store it in a VectorDB

## Instructions to run the model

1. **Install Dependencies**

Install the required packages using pip. The required packages are given in requirements.txt

2. **Add the YouTube links in linky.txt line by line:**

3. **Wait for Results:**
