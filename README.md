# Election AI Platform

Welcome to the **Election AI Platform**, a Streamlit application designed to provide election predictions and answer questions about political candidates through a chatbot powered by the Gemini AI model.

## Features

- **Election Predictions**: Analyze and predict the performance of election candidates based on provided data.
- **Political Chatbot**: Engage with a chatbot to ask questions about the election and candidates.
- **Data-Driven Insights**: The app uses uploaded election data in JSON format to generate predictions.
- **AI-Powered**: Utilizes the Gemini API for generating predictions and chatbot responses.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Arushan2/Election_agent
    ```

2. Navigate to the project directory:
    ```bash
    cd election-ai-platform
    ```

3. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your Gemini API key:

    You can choose to set the API key in one of two ways:

    ### Option 1: Environment Variable (default)
    Set the environment variable for the Gemini API key:
    ```bash
    export GEMINI_API_KEY='your_gemini_api_key_here'
    ```

    ### Option 2: Use `cred.py` (recommended for easier management)
    1. Create a file named `cred.py` in the project root directory.
    2. Add the following content to the `cred.py` file:
       ```python
       GEMINI_API_KEY = 'your_gemini_api_key_here'
       ```
    
    The application will check the `cred.py` file for the API key if the environment variable is not set.

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. You will be greeted with the home page offering two main options:
    - **Election Predictions**: Load election data from a folder and get AI-based predictions.
    - **Political Chatbot**: Ask questions to the AI chatbot about the candidates and election.

## Folder Structure

- `app.py`: Main file to run the Streamlit application.
- `cred.py`: Stores the Gemini API key if not set as an environment variable.
- `data1/`: Folder to upload or store election data in JSON format for predictions.
- `requirements.txt`: File containing the list of dependencies required for the project.



