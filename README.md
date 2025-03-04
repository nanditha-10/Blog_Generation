# Blog Generation using Llama 2 :

PROBLEM:
Writting a Blog is so hectic and after that correcting Grammatical errors is another Headache. Here comes the Solution. Blog Generator where you just need to specify the contents or just the topic name will work for you within 10 seconds!

DESCRIPTION :
We can generate any blog based on our given topic name, no. of words, blog style. we have used Llama 2 a open source llm model to build this Generative AI Project When you run it first time, it will take some time because to download of Model.


Internal Execution Flow (Step-by-Step):  

📌 Step 1: The user enters blog topic, word count, and audience type in Streamlit.

📌 Step 2: The app formats the input using LangChain’s PromptTemplate.

📌 Step 3: The LLama 2 model is loaded via CTransformers (or Replicate API).

📌 Step 4: The formatted prompt is sent to the model, which generates the blog.

📌 Step 5: The generated blog appears on the Streamlit page for the user to read.

<img width="396" alt="image" src="https://github.com/user-attachments/assets/f43b6f62-db66-4981-9a9d-2b94df56a87d" />


1. Web UI Framework → Streamlit
   
🔹 What It Does?

Streamlit is used to create the user interface (UI) for the app.
It allows users to input the blog topic, select word count, and choose a target audience (Researchers, Data Scientists, etc.).

2. Prompt Formatting → LangChain (PromptTemplate)

🔹 What It Does?

It helps format the input data into a structured prompt that the model can understand.
Instead of manually writing a string for the model, we use LangChain's PromptTemplate to format user input dynamically.

3. Model Execution → CTransformers (Llama 2 Model : TheBloke/Llama-2-7B-Chat-GGML)
   
🔹 What It Does?

It loads and runs the Llama 2 model to generate text based on the prompt.
CTransformers is a lightweight wrapper that allows running GGML-based models (like Llama 2) locally.

 4. Alternative Model API → Replicate API (Optional)
    
🔹 What It Does?

If running Llama 2 locally is slow or resource-intensive, we can use Replicate API to call a cloud-based Llama 2 model.
The Replicate API allows you to run AI models in the cloud without GPU dependency.








