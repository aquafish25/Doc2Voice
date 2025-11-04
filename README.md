# Doc2Voice

**Turn your PDFs, images or documents into spoken summaries - powered by state-of-the-art retrieval-augmented generation (RAG) and the DeepSeek model family.**

---

### 🔍 What it does  
This project provides an end-to-end pipeline that:
- Accepts a document in PDF (or an image with text)  
- Extracts and splits the text intelligently  
- Uses a retrieval-augmented generation (RAG) approach with the model DeepSeek‑R1‑Distill‑Qwen‑1.5B (and similar) to generate a concise summary  
  - The model family is trained for strong reasoning and was shown to perform impressively on math & logic benchmarks.
- Converts the summary text into speech using Google Text-to-Speech (`gtts`)  
- Outputs an audio file (e.g., MP3) you can listen to immediately  

### ⚙️ Features  
- Accepts image or PDF input  
- Text extraction via OCR (if image) or PDF parser  
- Smart text segmentation (splits large docs into manageable bits)  
- Retrieval based on semantic embeddings  
- Summarisation via large language model  
- Text-to-speech audio output  
- Easy to plug into other workflows (web apps, CLI, etc.)  

### Installation  
```bash
git clone https://github.com/YourUsername/Doc2Voice.git
cd Doc2Voice
pip install -r requirements.txt
