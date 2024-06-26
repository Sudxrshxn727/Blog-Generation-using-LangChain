# Blog Generation App

This project is a blog generation application built using Streamlit, Langchain, and the Llama-2-7b-chat-ggml model. The app allows users to generate blogs by specifying the topic, blog style, and the desired word count. 

## Features

- **Topic Input**: Users can input the topic they want the blog to be about.
- **Blog Style**: Users can select the style of the blog - whether it is meant for common people, data scientists, or researchers.
- **Word Count**: Users can specify the number of words for the blog.
- **Generate Button**: A button to generate the blog based on the provided inputs.

## Installation

### Prerequisites

- Python 3.8 or higher
- Streamlit
- Langchain
- CTransformers
- Llama-2-7b-chat-ggml model

### Steps

1. **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Install the required libraries**:
    ```bash
    pip install streamlit langchain ctransformers
    ```

3. **Download the Llama-2-7b-chat-ggml model**:
    - Visit [Hugging Face](https://huggingface.co/) to download the Llama-2-7b-chat-ggml model.
    - Save the model in a directory on your local machine.

4. **Run the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

## Usage

1. Open the Streamlit app in your browser.
2. Enter the topic of the blog.
3. Select the blog style from the dropdown (common people, data scientists, researchers).
4. Specify the number of words for the blog.
5. Click on the "Generate" button to generate the blog.

## Code Overview

### Imports

```python
import streamlit as st
from langchain.prompts import PromptTemplate
from langchain.llms import CTransformers
```

### Streamlit UI

- **Topic Input Field**: A text input field for the topic.
- **Blog Style Dropdown**: A dropdown menu to select the blog style.
- **Word Count Input Field**: A number input field for specifying the word count.
- **Generate Button**: A button to generate the blog.

### Prompt Template

The prompt template is defined with three input fields:

- `topic`: The topic of the blog.
- `blog_style`: The style of the blog (common people, data scientists, researchers).
- `no_of_words`: The number of words for the blog.

### Blog Generation

When the "Generate" button is clicked, the app uses the Llama-2-7b-chat-ggml model to generate the blog based on the provided inputs.

## Conclusion

This Blog Generation App provides an easy way to generate blog content based on user inputs. By leveraging the power of Streamlit, Langchain, and the Llama-2-7b-chat-ggml model, the app delivers a seamless experience for creating customized blog content.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements

- [Streamlit](https://streamlit.io/)
- [Langchain](https://langchain.com/)
- [Hugging Face](https://huggingface.co/)

Feel free to contribute to this project by opening issues or submitting pull requests. Happy blogging!
