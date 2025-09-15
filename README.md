# CodeVirt

**CodeVirt** is a Go-based AI-powered tool that converts handwritten code into executable programs.  
Upload an image of handwritten code, and CodeVirt extracts the text, executes it securely inside a Docker container, and returns the output — all in a streamlined workflow.

---

## 🚀 Features

- 📝 **Handwritten Code Recognition** – Extract code from images with preprocessing and OCR.  
- ⚡ **Secure Code Execution** – Run Python code safely inside ephemeral Docker containers.  
- 🌐 **REST API** – Simple endpoints for uploading images and executing code.  
- 🎨 **GUI / Web Frontend (Future)** – Planned desktop (Fyne) or web interface for easy interaction.  
- 🔒 **Sandboxed Environment** – Containers isolate execution to prevent security risks.  
- 🔮 **Extensible Architecture** – Designed to add multi-language support and AI-assisted error correction.

---

## 📂 Project Structure
codevirt/
├── cmd/ # Entry point
│ └── main.go
├── internal/
│ ├── api/ # REST endpoints
│ ├── ocr/ # OCR logic
│ ├── exec/ # Docker code execution
│ └── preprocess/ # Image preprocessing (GoCV)
├── go.mod
└── go.sum


---

## 🛠️ Prerequisites

- Go 1.22+ ([Download](https://go.dev/dl/))  
- Docker ([Download](https://www.docker.com/get-started)) running locally  
- Optional: OpenAI or Anthropic API credentials for modern OCR  

---

## 💻 Installation

```bash
# Clone the repo
git clone https://github.com/yourusername/codevirt.git
cd codevirt

# Install dependencies
go mod tidy


