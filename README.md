# OpenAI-Chroma-Langchain
This repo contains an use case integration of OpenAI, Chroma and Langchain


In simpler terms, prompts used in language models like GPT often include a few examples to guide the model, known as "few-shot" learning. To make these prompts more relevant, examples can be automatically pulled from a database using a special process called document retrieval. This often involves using a vector database.

Here's how it works: When you have a question (query), a document retriever tool searches for the most relevant documents. It does this by converting both your question and the documents into mathematical representations called vectors. The documents whose vectors are closest to your query's vector in a mathematical space (measured using something called Euclidean norm) are considered the most relevant.

Once the relevant documents are retrieved, the language model (like GPT) uses both your original question and the information from these documents to generate an answer. This approach is particularly useful for getting information that is unique, constantly changing, or was not included when the model was initially trained or fine-tuned.

![image](https://github.com/ParthaPRay/OpenAI-Chroma-Langchain/assets/1689639/a3750b42-d0c7-4324-996d-cb643cc989c9)


# LLM Used

**gpt-3.5-turbo-instruct**

# LLM Chain

**Langchain**

![download](https://github.com/ParthaPRay/OpenAI-Chroma-Langchain/assets/1689639/95697336-c859-48b0-9a3a-2392d3a85655)


# Vector Database

**chroma**  ![download](https://github.com/ParthaPRay/OpenAI-Chroma-Langchain/assets/1689639/fb4b4a99-592c-4eb5-b839-83e7d61dd8a3)


# Instructions


1. Open the Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ParthaPRay/OpenAI-Chroma-Langchain/blob/main/opeai_chroma_langchain.ipynb)


2. Change 'ENTER YOUR API KEY' to your own OpenAI API key


```python
os.environ['OPENAI_API_KEY'] = 'ENTER YOUR API KEY'
```


3. Upload the 'iot.txt' to /content folder of Google Colab as shown beow:
   

![Screenshot 2024-01-04 122039](https://github.com/ParthaPRay/OpenAI-Chroma-Langchain/assets/1689639/765a3686-fced-4acf-a693-ceb53e3bd8fb)



# Libraries

* langchain

* h11 

*httpcore 

* httpx

* openai

* sentence-transformers

* chromadb



References

1. https://www.youtube.com/watch?v=tXnpnnA4D5A&ab_channel=PythonAI

2. https://gist.github.com/SandyLudosky/ceafa0a12fbf620c56034db3c877eae5

3. https://en.wikipedia.org/wiki/Prompt_engineering
