# Hugging Face

`https://huggingface.co/docs/transformers/en/installation`


Hugging Face is a leading AI company and open-source platform that provides tools, models, and libraries for natural language processing (NLP), computer vision, and other machine learning tasks. It is best known for its "Transformers" library, which simplifies the use of pre-trained models like BERT, GPT, T5, and CLIP, making them accessible for tasks such as text classification, translation, summarization, and image recognition.

## 🔹 Hugging Face Task
A **task** is the type of AI problem a model is trained to solve.  
Examples:
- **Text Classification** – sentiment analysis, topic detection  
- **Token Classification** – named entity recognition (NER)  
- **Text Generation** – chatbots, autocomplete  
- **Machine Translation** – translating text  
- **Image Classification**, **Object Detection**, **Speech Recognition**, etc.  

When choosing a model on Hugging Face, you usually filter by its **task**.

---

## 🔹 Hugging Face Hub
The **Hub** is a platform (like GitHub for AI) where you can:
- Discover and use pre-trained **models**  
- Share your own models and **datasets**  
- Explore interactive **Spaces** (apps built with Gradio/Streamlit)  
- Access everything via API or the `huggingface_hub` Python library  

---

👉 In short:
- **Task** = what the model does  
- **Hub** = where models, datasets, and apps live



# Transformers

**Transformers** is an open-source library by Hugging Face.  
It provides **pretrained models** and tools for NLP, computer vision, and audio tasks, built on the **Transformer architecture** (used in BERT, GPT, T5, ViT, etc.).

---

## Key Features
- Easy access to models from the **Hugging Face Hub**  
- Simple inference with `pipeline()`  
- Supports **PyTorch, TensorFlow, and JAX**  
- Fine-tuning utilities (`Trainer`, `AutoModel`, `AutoTokenizer`)  

---

