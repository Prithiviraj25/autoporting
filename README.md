# **AUTO-PORTING TOOL**
***
## **Initial Data Preparation**
The initial step involves utilizing the repositories of tools that have already been ported for the ZOs Operating System. Using the ZOs environment, we will proceed by removing all patch codes, then rebuild the tool. Subsequently, patches will be added one by one, and errors encountered during each addition will be captured for further analysis.

The dataset is structured in the following format:
```json
{
  "wrong_code": "",
  "error_category": "",
  "error": "",
  "correct_code": "",
  "patch": ""
}
```

* wrong_code: The code segment that caused the error.
* error_category: The category or type of the error.
* error: The specific error message or description encountered.
* correct_code: The modified or correct code that resolves the error.
* patch: The patch applied to the code.
  
for each and every error the above format is followed and the data is captured.
This format ensures clear tracking of errors, their categories, and the corresponding fixes.
***
## **Selecting the Appropriate Model**
* To install the Instruct Lab, ensure that **Python 3.9.20** is used, as this version is compatible for hosting the external model.
  Please go through the documentation of Instruct Lab for the installation [Instruct Lab Documentation](https://docs.instructlab.ai/)
* The selected model, **deepseek-coder-1.3b-instruct_Q4_0**, is an advanced deep learning model designed for code-related tasks. It is based on the GPT architecture and trained on large datasets tailored for programming and software development. The model is capable of understanding, generating, and assisting with code in various programming languages.
  Please visit the website for further information on the model used [link](https://huggingface.co/TheBloke/deepseek-coder-1.3b-instruct-GGUF)
***
## **Synthetic Data Generation**
