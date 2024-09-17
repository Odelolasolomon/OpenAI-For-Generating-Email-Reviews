# OpenAI API Image and Text Generation Project

This project demonstrates the use of the OpenAI API for various image and text generation tasks. The tasks include email generation based on Amazon reviews, code generation, text summarization, and image generation using OpenAI’s models.

## Project Overview

The project involves:

- **Email Generation**: Create personalized emails based on Amazon reviews using GPT-3.5.
- **Code Generation**: Write code snippets using GPT-3.5.
- **Text Summarization**: Summarize extracted text from a PDF using GPT-3.5.
- **Image Generation**: Generate images based on prompts using DALL-E 3.

## Set Up the Environment

### Create a Virtual Environment (optional but recommended)

```bash```
- python -m venv venv

## Install the Required Packages
- pip install -r requirements.txt

## Set Up the Configuration
- Create a .env File

## Running the Application
- Start the Flask Development Server
- flask run --host=0.0.0.0

## File Structure
- app.py: Core file that executes the Flask application.
- website/: Contains the main application code and templates.
- __init__.py: Configures the Flask application and database.
- models.py: Defines the database models.
- routes.py: Manages the routes and view functions.
- templates/: Contains HTML templates.
- base.html: Base template with navbar and layout.
response_view.html: Displays responses from GPT-3.
- history.html: Displays the history of interactions.

## Contributing
- Feel free to open issues or submit pull requests. Contributions are welcome!

## License
- This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Flask: A lightweight WSGI web application framework for Python.
- OpenAI: Provides the GPT-3 API for generating responses.
- Bootstrap: Frontend framework used for styling.

## Jupyter Notebook Instructions
- Task 1: Import Modules and Packages
- Load the following modules and packages:
- openai: Used for accessing the OpenAI API.
- pandas: Used for handling tabular data.
- requests: Used for downloading files.
- datetime from datetime: Required for getting the timestamp.
- pprint from pprint: Required for pretty printing text in Python.
- tiktoken: Required for counting the number of tokens in a string.
- PdfReader from pypdf: Required for handling PDF files.
- Markdown, and display from IPython.display: Required for loading and displaying markdown content in the notebook.
- os: Required to access operating system resources.
- pyplot and image from matplotlib: Required for displaying images in the notebook.

## Task 2: Get OpenAI API Key
- Get your OpenAI API key by following the instructions given in the Educative Answer, “How to get API Key for GPT-3.”

## Task 3: Email Generation
- Run the first cell to create a pandas DataFrame containing reviews from various subsets of the Amazon reviews dataset.
- Write a function to generate an email to the customer when a review is provided as input.
- Create a chat transcript with roles system, user, and assistant.
- Append a line instructing the assistant to generate an email to address the user’s issues.
- Use client.chat.completions.create() to generate a response from the API.
- Populate the emails column in the DataFrame using the function and DataFrame.apply().
- Pretty-print the DataFrame using the pp() method.
- 
##Task 4: Code Generation
- Run the first cell to create a list of problems for which you need to write code.
- Create a chat transcript with the instructions to generate Python code for each problem.
- Generate a response from the API.
- Print the problem name capitalized and use display() and Markdown() to display the API response in markdown.

## Task 5: Text Summarization
- Run the first cell to:
- Create a function that computes the number of tokens in a string.
- Download a research paper PDF using the requests library.
- Extract the content and save it as a string.
- Compute the number of tokens in the string.
- Create a chat transcript with instructions to generate a summary.
- Generate a response from the API.
- Display the summary in markdown using display() and Markdown().
- Get the number of tokens in the summary.

## Task 6: Image Generation
- Repeat the following steps for the desired number of images:
- Generate an image using client.images.generate() with parameters:
- model: The model to use.
- prompt: Description of the image to generate.
- size: Image size (e.g., 1792x1024, 1024x1792, 1024x1024).
- quality: standard or hd.
- n: Set to 1.
- Use display() and Markdown() to display the reworded prompt.
- Use the requests library to download the image and save it locally.
- Display the generated image in the notebook.
