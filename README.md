# **Targeted Keyword Discovery for Class-Based Document Categorization**

## **Overview**
This project presents a refined approach to keyword extraction tailored for specific classes or categories of documents. Building on the KEYBERT algorithm, our method leverages advanced NLP techniques to identify class-specific keywords with high precision, making it ideal for applications like document classification and topic modeling.

## **Key Features**
- **Class-Specific Keyword Extraction:** Focuses on domain-relevant keywords, ensuring precise categorization.
- **Iterative Refinement:** Uses cosine similarity to enhance keyword relevance iteratively.
- **Scalable and Efficient:** Handles large datasets effectively with mid-range computational resources.
- **Multi-Algorithm Support:** Integrates methods like TextRank, RAKE, and TF-IDF for diverse keyword extraction.
- **Robust Evaluation:** Tested on the German Handelsregister dataset with significant performance improvements over traditional methods.

## **Project Structure**
- **Data Ingestion:** Automates data collection and preprocessing for structured and unstructured inputs.
- **Keyword Extraction:** Implements enhanced keyword extraction using embedding-based scoring.
- **Classification Module:** Categorizes documents into predefined classes using rule-based and machine-learning models.
- **User Interface:** A Streamlit-based application for uploading, processing, and exporting document analysis results.
- **Evaluation Metrics:** Includes precision, recall, and F1-score to assess performance.

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name
   cd your-repo-name
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## **Usage**
1. Run the Streamlit application:
   ```bash
   streamlit run main.py
   ```
2. Access the application in your browser at `http://localhost:8501`.
3. Upload a `.docx` or `.pdf` file for keyword extraction.
4. Process and export the results in your preferred format (PDF or Word).

## **Dataset**
- **Source:** German Business Registry (Handelsregister)
- **Entries:** 10,000 records classified based on the WZ 2008 economic classification scheme.

## **Results**
- **Precision@10:** 28.10% (compared to 2.38% with guided KEYBERT).
- **Cosine Similarity:** Achieved an average match rate of 85% or higher.
- **Performance:** Outperformed RAKE, YAKE, and standard KEYBERT in class-specific keyword extraction.

## **Future Directions**
- Extend support for multi-word keyphrase extraction.
- Adapt the method for multilingual datasets.
- Optimize the iterative refinement process for greater computational efficiency.
- Validate real-world deployment in domains like healthcare, e-commerce, and legal.

## **Acknowledgements**
Special thanks to our supervisor, **Dr. Iyappan P**, and the School of Computer Science and Engineering, VIT, for their guidance and support throughout this project.

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for more details.

