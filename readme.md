How To Run
Follow the steps below to set up and run your Retrieval-Augmented Generation (RAG) system:

### 1. **Install Necessary Libraries**

Before running the code, ensure that all the required libraries are installed in your environment.

- If you have a `requirements.txt` file that lists all the dependencies, you can install the necessary libraries by running this command in your terminal or command prompt:

  ```bash
  pip install -r requirements.txt
This will automatically install all the libraries and their required versions as specified in the requirements.txt file.

If you don’t have a  `requirements.txt`, you will need to manually install the libraries, such as transformers, torch, faiss, sentence-transformers, etc., depending on your specific project needs.
### 2. Add Documents to the `./data/` Folder
The RAG system needs documents to perform the retrieval step. These documents should be placed in the `./data/` folder in your project directory.

How to structure the folder:
Create a folder named data inside your project directory.
Add your documents (text files, PDFs, or any other supported format) to the data folder.
Example directory structure:

```
project_directory/
├── data/
│   ├── document1.txt
│   ├── document2.pdf
│   └── document3.txt
├── requirements.txt
├── test.ipynb
└── ...
```
Supported Document Formats:
You can use `.txt` for plain text, `.pdf` for PDF documents, or any other format supported by the document processing functions in your project.
If you’re working with PDF files, ensure that the appropriate library (like `PyMuPDF`, `pdfminer`, or `PyPDF2`) is available in your environment to extract text.
### 3. Set Your Query in the queryy Variable
In the code, you will need to define the query you want to process. The variable queryy should hold the text of your query.

Open the test.ipynb notebook in Jupyter Notebook or any other environment that supports .ipynb files.

Locate the section where the query is defined and set the queryy variable to your desired query.

Example:
```
queryy = "What are the key features of RAG models?"
The queryy variable is the input query for the RAG model, and it will be used to retrieve relevant documents from the ./data/ folder and then generate an answer based on the content.
```
### 4. Run the Code Blocks in test.ipynb
Once you have your environment set up, documents added, and the query set, you can begin running the code blocks in the test.ipynb notebook.

In the Jupyter interface, navigate to your project folder and open the test.ipynb file.
Running the Code Blocks:

In the Jupyter Notebook, run each code block sequentially. You can run blocks by clicking on the cells and pressing Shift + Enter or using the "Run" button.
The notebook will first load the necessary libraries, process the documents from the `./data/` folder, perform the retrieval step, and generate an answer based on the query.

Answer Generation: A generative model (Groq AI) will then generate an answer based on the retrieved documents.

