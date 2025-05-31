## 🧠 Simple Guide to Load LLaMA 3.2 with QLoRA

This notebook provides a **minimal and effective setup** to load **Meta's LLaMA 3.2–8B** using **QLoRA** (4-bit quantization). No modifications are made — it's the original model, fully configurable for your own use cases.

---

### ✅ Instructions

1. **Create or log in** to your [Hugging Face](https://huggingface.co/) account  
2. **Generate a Hugging Face Access Token**  
   → Go to: `https://huggingface.co/settings/tokens`  
3. Paste the token into the code (where prompted) or use secure loading (see “Token Security” below)  
4. Run the notebook to load the model with **4-bit quantization (QLoRA)**

---

### 💻 System Requirements

- QLoRA uses **quantized 4-bit loading**, which **only works on Linux-based systems**
- You can:
  - ✅ Use **native Linux** (recommended for speed)
  - ✅ Or run via **WSL Ubuntu** on Windows (slower but works)

---

### 🔐 Token Security

**Never hardcode your Hugging Face token in public notebooks.**  
Use one of the following methods:

```bash
# Recommended CLI method
pip install huggingface_hub
huggingface-cli login
