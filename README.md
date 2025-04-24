# GenAI Capstone – Multimodal Intelligence Demonstration

This project is a demonstration of multimodal artificial intelligence powered by **Google’s Gemini** model. It explores how large language models can effectively understand and interact with **documents, images, and audio**, while also utilizing advanced prompting techniques like **few-shot learning**, **JSON parsing**, and **function calling** to create dynamic and intelligent responses.

## Project Goals
- Demonstrate Gemini’s multimodal understanding capabilities.
- Showcase prompt engineering for structured and flexible interactions.
- Build a modular, reusable pipeline for AI-assisted tasks.

---

## Key Features

### Document Understanding
- **Library Used**: `PyMuPDF (fitz)`
- **Functionality**: Extracts raw text from PDFs (e.g., _A Brief History of Time_).
- **Model Task**: Summarize content and highlight key learnings.
- **Learning Outcome**: Structuring long-form prompts for summarization.

---

### Image Processing
- **Image Source**: A Bob Ross painting.
- **Display Method**: `IPython.display.Image`
- **Model Task**: Describe the image in detail with emotional context.
- **Learning Outcome**: Prompting for visual and perceptual analysis.

---

### Audio Understanding
- **Input**: Audio file containing spoken content.
- **Model Task**: 
  - Transcribe the speech  
  - Summarize the message  
  - Detect speaker intent
- **Output**: JSON-formatted response.
- **Learning Outcome**: Structured multimodal prompts and audio comprehension.

---

### Few-Shot Prompting
- **Task**: Convert natural language instructions into Python functions.
- **Technique**: Few-shot learning with syntactic and semantic patterning.
- **Learning Outcome**: Example-driven prompt crafting.

---

### JSON Parsing
- **Task**: Post-process model responses.
- **Tools Used**: `json.loads()` with markdown cleaning.
- **Learning Outcome**: Reliable parsing of structured model outputs.

---

### Function Calling
- **Custom Helper**: `display_transcript()`
- **Purpose**: Selectively display fields like transcript, summary, or intent.
- **Learning Outcome**: Modular access to model responses for better reuse.

---

## Tech Stack

| Component        | Tool/Library            |
|------------------|-------------------------|
| Language Model   | Google Gemini (via API) |
| PDF Parsing      | PyMuPDF (`fitz`)        |
| Image Handling   | IPython Display         |
| JSON Processing  | Python `json` module    |
| Notebook Format  | Jupyter / Kaggle        |

---

## Setup & Usage

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/genai-capstone.git
   cd genai-capstone
   ```
   
2. Run the notebook on Kaggle or locally using Jupyter Lab::
   ```
   pip install -r requirements.txt
   ```
   
3. Get Your Gemini API Key
   -- Head over to [Google AI studio](https://aistudio.google.com/) and grab an API key
   -- Add it as a Kaggle Secret or environment variable GOOGLE_API_KEY.

---

## Future Enhancements

- Integrate video understanding.

- Expand function-calling capabilities (e.g., database queries).

- Build a simple front-end UI for user interaction.
