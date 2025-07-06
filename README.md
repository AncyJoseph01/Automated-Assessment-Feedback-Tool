# Automated Assessment Feedback Tool

**This project uses the meta-llama/Llama-3.1-8B-Instruct model** to generate structured feedback for question-and-answer pairs extracted from a Word document (Q1.docx). The feedback is then added as comments to the same document. It is designed to provide automated, structured feedback on responses.

##**Features**

*   **Extracts Q&A:** Reads question-answer pairs from a Word document.
*   **Generates Feedback:** Uses LLaMA 3.1 via Hugging Face's InferenceClient to produce structured feedback (positive points, praise, and suggestions for improvement).
*   **Adds Comments:** Inserts feedback as comments in the original Word document.
*   **Saves Output:** Updates the input document with feedback comments.

##**Prerequisites**

*   Python 3.8+
*   A Hugging Face account with an API token for accessing the LLaMA model.
*   A Word document (Q1.docx) with Q&A pairs formatted as Q1., Q2., etc., for questions and A1., A2., etc., for answers.

##**Usage**
*   Prepare the Input Document:
    *    Create a Word document (Q1.docx) with Q&A pairs. Example format:

    Q1. What is the safeguarding policy?

    A1. The policy ensures safety and compliance.
    
    Q2. How is safeguarding implemented?

    A2. Through training and regular audits.

##**Run the Notebook**
*   Open Comment_Project.ipynb in a Jupyter environment (e.g., Google Colab, JupyterLab).
*   Execute all cells to:
   *   Install dependencies.
   *   Extract Q&A pairs from Q1.docx.
   *   Generate feedback using LLaMA 3.1.
   *   Add feedback as comments to Q1.docx.

## **Output**
*   The modified Q1.docx will contain feedback as comments for each question.
*   Example feedback format:
   *   ✅ Positive points: Clear explanation of the policy.
   *   👏 Praise: Well-structured response.
   *   ⚠️ Suggestions for improvement: Include specific examples to strengthen the answer.



---

