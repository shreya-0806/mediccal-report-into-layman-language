# 🏥 Medical Report to Patient-Friendly Summary Generator

This project transforms complex clinical documents such as discharge summaries and medical notes into simplified, patient-friendly summaries. Using advanced AI and NLP tools, it identifies diseases, symptoms, and prescribed medications, then explains them in a way that non-medical individuals can easily understand.

> 📍 **Summer Training Bootcamp Project**  
> 🎓 **Institution:** SRMCEM, Lucknow  
> 💡 **Internship Theme:** Artificial Intelligence  
> 👨‍💻 **Team Members:**  
> - [Shreyanshi Srivastava](https://github.com/shreya-0806)  
> - [Sarthak Pandey](https://github.com/spcodes26)  
> - Shubham Kumar  

[🔗 Open Project on Google Colab](https://colab.research.google.com/drive/1F0ax9YSadvLe1ZiGNKosFL1MhZYTpglr?usp=sharing)

---

## 📘 Project Topic

**"AI-Powered Clinical Report Simplifier"**  

***Medical report to patient-Friendly Summary Generator....***
 Input PDF: Clinical notes, medical research papers or discharge summaries
 Output task : Generate a layman-understandable explanation of a patient(e.g. , what disease, symptoms, prescribed medicines).
 
The goal is to make medical reports understandable for patients by converting technical medical text into easy-to-read summaries using AI.

---

## 🧰 Libraries and Tools Used

- **pdfplumber** – Extracts text from medical PDF files.
- **sentence-transformers** – Converts sentences into numerical vectors (embeddings).
- **faiss-cpu** – Performs fast similarity search over text embeddings.
- **transformers** – Access to pre-trained models like Pegasus for summarization.
- **google/pegasus-xsum** – A transformer model fine-tuned for abstractive summarization.
- **gradio** – Provides a simple and interactive UI for users to upload files and view output.
- **numpy** – Handles numerical operations for embeddings.

---

## 🧭 Project Workflow

1. **Upload PDF**: The user uploads a clinical report (e.g., discharge summary).
2. **Text Extraction**: Extract raw text using `pdfplumber`.
3. **Text Chunking & Embedding**: Split the text and convert it into embeddings using Sentence Transformers.
4. **Semantic Search**: Use FAISS to find relevant content for each predefined question (disease, symptoms, medicines).
5. **Summarization**: Generate layman-friendly summaries using the Pegasus XSum model.
6. **User Interface**: Display final output using Gradio.

---

## ✅ How to Use

1. Open the [Google Colab notebook](https://colab.research.google.com/drive/1F0ax9YSadvLe1ZiGNKosFL1MhZYTpglr?usp=sharing).
2. Upload any medical PDF (like a discharge summary).
3. Let the app process and extract the necessary information.
4. View the simplified summary in a readable format.

---

## 📌 Input & Output Example

**Sample PDF Input**:
- **Diagnosis**: Type 2 Diabetes
- **Symptoms**: Frequent urination, fatigue
- **Medications**: Metformin

**Patient-Friendly Output**:
> 🔹 **Disease/Condition**: You have Type 2 Diabetes, which affects blood sugar levels.  
> 🔹 **Symptoms**: You might feel tired often and need to urinate frequently.  
> 🔹 **Medications**: You’re prescribed Metformin to control blood sugar.

---

## 🚀 Future Enhancements

- Support for scanned or handwritten reports via OCR.
- Multi-language summaries (e.g., Hindi, Bengali).
- Downloadable or email-ready summary formats.
- Integration with a chatbot for question-based interaction.

---

## 📑 License

This project was developed for academic purposes as part of SRMCEM’s Summer AI Bootcamp 2025. All code and methods are for educational use.

---

## 👥 Contributors

- [**Shreyanshi Srivastava**](https://github.com/shreya-0806) – Lead, Gradio UI, Summarization  
- [**Sarthak Pandey**](https://github.com/spcodes26) – PDF Extraction, Embeddings  
- **Shubham Kumar** – FAISS Search, Optimization  

---

