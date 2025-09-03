# AI Article Assistant

This project demonstrates how to use **LangChain** to create an AI assistant that helps with writing articles.  
The assistant can:  
- Generate a catchy **title**  
- Write an **SEO-friendly description**  
- Provide **feedback on a paragraph** with suggested edits  

---

## 🚀 Setup

1. **Install Dependencies**  
   Run the first cell to install the necessary libraries.

2. **Set up OpenAI API Key**  
   Run the second cell to set up your OpenAI API key.  
   You will be prompted to enter your key.

3. **Initialize Language Models**  
   Run the third cell to initialize the `ChatOpenAI` models with and without temperature for different response styles.

---

## 📝 Code Explanation

- **Cell 4**: Contains the article text that will be used as input for the AI assistant.  
- **Cells 5–7**: Define the prompt for generating the **article title** and create a **LangChain Expression Language (LCEL)** chain to invoke the language model and extract the title.  
- **Cells 9–11**: Define the prompt for generating the **article description** and create an LCEL chain to invoke the language model and extract the description.  
- **Cells 13–16**: Define the prompt for reviewing and editing a **paragraph**, define a **Pydantic model** for the structured output, and create an LCEL chain to invoke the language model with structured output.  
  This extracts:
  - Original paragraph  
  - Edited paragraph  
  - Feedback  

---

## ▶️ Usage

1. Run all the code cells in the notebook.  
2. The outputs of the last three chains will contain:  
   - `chain_one` → Generated **article title**  
   - `chain_two` → Generated **article description**  
   - `chain_three` → **Paragraph review** with edits & feedback  

---
