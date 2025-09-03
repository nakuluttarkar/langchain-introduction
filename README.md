##AI Article Assistant
This project demonstrates how to use LangChain to create an AI assistant that helps with writing articles. The assistant can generate a catchy title, an SEO-friendly description, and provide feedback on a paragraph with suggested edits.

##Setup
Install Dependencies: Run the first cell to install the necessary libraries.
Set up OpenAI API Key: Run the second cell to set up your OpenAI API key. You will be prompted to enter your key.
Initialize Language Models: Run the third cell to initialize the ChatOpenAI models with and without temperature for different response styles.
##Code Explanation
Cell 4: Contains the article text that will be used as input for the AI assistant.
Cells 5-7: Define the prompt for generating the article title and create a LangChain expression language (LCEL) chain to invoke the language model and extract the title.
Cells 9-11: Define the prompt for generating the article description and create an LCEL chain to invoke the language model and extract the description.
Cells 13-16: Define the prompt for reviewing and editing a paragraph, define a Pydantic model for the structured output, and create an LCEL chain to invoke the language model with structured output and extract the original paragraph, edited paragraph, and feedback.
Usage
Run all the code cells in the notebook.
The outputs of the last three chains (chain_one, chain_two, and chain_three) will contain the generated article title, description, and the paragraph review with feedback, respectively.
