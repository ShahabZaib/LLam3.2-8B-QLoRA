# 🧠 Simple Guide to Load LLaMA 3.2 with QLoRA

This notebook provides a **minimal and effective setup** to load Meta's **LLaMA 3.2–8B Instruct** model using **QLoRA** (4-bit quantization). No modifications are made — it’s the original model, fully configurable for your own tasks.

---

## ✅ Setup Instructions

1. **Log into your Hugging Face account**  
2. **Generate a Hugging Face Access Token**  
   → https://huggingface.co/settings/tokens  
3. **Paste your token** in the notebook where prompted — or use secure loading (see below)  
4. **Run the notebook** to load the model using 4-bit QLoRA  

---

## 💻 System Requirements

QLoRA requires **Linux-based environments** to load 4-bit quantized models. You can:

- ✅ Use **native Linux** (recommended)
- ✅ Or run via **WSL Ubuntu** on Windows (slightly slower, but works fine)

---

## 🔐 Token Security

Never hardcode your Hugging Face token.

Use either of the secure methods below:

### Method 1: CLI Login

    pip install huggingface_hub
    huggingface-cli login

### Method 2: Use `.env` (Optional)

1. Create a file named `.env`:

    HF_TOKEN=your_token_here

2. Load it in Python:

    from dotenv import load_dotenv
    import os

    load_dotenv()
    token = os.getenv("HF_TOKEN")

---

## 📂 Included Files

- `Load_LLaMA3_QLoRA.ipynb`: Notebook for loading and testing the model  
- `.gitignore`: To ignore model paths, cache, tokens, etc.  
- `LICENSE`: MIT License  
- `requirements.txt`: Required packages  

---

## 📦 Requirements

Install all dependencies with:

    pip install -r requirements.txt

Or manually:

    pip install transformers accelerate peft bitsandbytes huggingface_hub

---

## 📝 License

MIT License – free to use, modify, and share with credit.
