# VidyaSetu – A LLM-Powered Knowledge Bridge for Hindi (Ongoing)

## Overview  
VidyaSetu is an educational assistant that helps bridge the gap between English queries and Hindi learning content. The project combines language models, retrieval systems, and text-to-speech so that students can ask questions in English and get clear answers in Hindi (as text or audio).  

The aim is to make NCERT, GK, and other educational material more accessible in Hindi, and eventually extend this to other Indian languages.  

---

## Problem Statement  
Most AI assistants are designed for English. For Hindi learners, there are fewer tools that provide:  
- Domain-specific answers (NCERT, exams, GK)  
- Proper bilingual support  
- Natural-sounding speech  

VidyaSetu tries to solve this using a LoRA fine-tuned model, Retrieval-Augmented Generation (RAG), and Hindi TTS.  

---

## Objectives  
- Take questions in English and return answers in Hindi.  
- Fine-tune models on educational data for better relevance.  
- Use a vector database (FAISS/ChromaDB) for context retrieval.  
- Provide answers as both text and audio.  
- Keep the design modular so it can be extended to other Indic languages.  

---

## Current Progress  
- ✅ Working GPT-2 prototype (English QA → Hindi translation → speech).  
- ✅ Integrated Google Translate + gTTS for testing.  
- 🔄 Setting up LoRA fine-tuned models for domain-specific answers.  
- 🔄 Adding RAG pipeline with ChromaDB/FAISS.  
- 🔄 Flask UI in progress for query + response display.  

---

## Tech Stack  
- Python, Flask  
- PyTorch, Hugging Face Transformers  
- LoRA fine-tuning (PEFT)  
- ChromaDB / FAISS (retrieval)  
- gTTS / IndicTTS for audio  

---

## Workflow  
1. User enters a question in English  
2. Model processes and generates answer (English → Hindi)  
3. Context added through retrieval (NCERT/GK)  
4. Hindi text returned + converted to audio  
5. User receives text and/or speech output  

---

## Challenges  
- Fine-tuning needs GPUs and good datasets  
- Retrieval indexing is critical for accuracy  
- TTS for Indic languages can be slow or less natural  
- Integrating LLM + RAG + TTS into one smooth pipeline  

---

## Expected Outcomes  
- Functional assistant that answers Hindi queries from English input  
- Context-aware and more accurate than plain translation  
- Text + audio delivery for accessibility  
- Base for scaling to other Indic languages  

---

## Repository Structure (planned)  
```
VidyaSetu/
│── app/           # Flask app
│── models/        # Fine-tuned weights / tokenizer
│── rag/           # Retrieval module
│── tts/           # Text-to-speech integration
│── notebooks/     # LoRA fine-tuning + experiments
│── docs/          # Diagrams, workflow
│── README.md
```

---

## Future Scope  
- Add Kannada, Tamil, Telugu support  
- Multimodal (text + images) explanations  
- Deploy on cloud for real-time usage  

---

## Skills Involved  
- LLM fine-tuning (LoRA)  
- Retrieval-Augmented Generation (RAG)  
- Bilingual NLP (English ↔ Hindi)  
- Flask backend integration  
- TTS pipeline setup  

## Curent ouput
<img width="587" height="402" alt="Screenshot 2025-08-26 235925" src="https://github.com/user-attachments/assets/3c2a37c2-9115-4f86-b6b0-43e699bf7e76" />


<h2 id="contact">Contact</h2>
  <p>For any inquiries or feedback, please contact:</p>
  <ul>
    <li><strong>Name:</strong> Deepanshu Miglani</li>
    <li><strong>Education:</strong> B.tech CSE(AIML) , UPES, Dehradun</li>
    <li><strong>Email:</strong> deepanshumiglani0408@gmail.com / Deepanshu.106264@stu.upes.ac.in</li>
    <li><strong>GitHub:</strong> <a href="https://github.com/deepanshum0408">deepanshum0408</a></li>
  </ul>
