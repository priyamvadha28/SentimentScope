# SentimentScope
SentimentScope is a Python-based sentiment analysis tool that leverages Azure OpenAI's language model (LLM) to analyze and categorize client feedback. The project is designed to process feedback data from various Excel files, clean the text, and classify the sentiment into categories: "progressive," "lagging," "stagnant," or "unclear." Each feedback entry is evaluated for sentiment and assigned a score between 0 and 100 along with a reason for the classification.

Features:
- Text Cleaning: Removes non-ASCII characters, extra whitespace, and formatting issues from the feedback text.
- Sentiment Classification: Categorizes feedback into "progressive," "lagging," "stagnant," or "unclear" based on its content.
- LLM Integration: Uses Azure OpenAI’s language model to analyze and interpret the sentiment of feedback.
- Result Storage: Outputs the sentiment analysis results to an Excel file for easy review and interpretation.

Setup:

1. Clone the Repository:
git clone <repository-url>

2. Navigate to the Project Directory
cd <repository-directory>

3. Install Dependencies
Create a virtual environment (optional but recommended) and install the required packages:
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt

4. Configure Azure OpenAI:
Set up your Azure OpenAI API key and endpoint in the script. Replace the placeholders in the AZURE_OPENAI_API_KEY and AZURE_OPENAI_ENDPOINT variables with your credentials.

Usage:

1. Prepare Your Dataset:
Ensure your Excel file contains feedback data with relevant columns. Update the file path in the script to point to your dataset.

2. Run the Script:
Execute the Python script to perform sentiment analysis:
python sentiment_analysis.py

The script will process the feedback, analyze the sentiment, and save the results in an Excel file named sentiment_analysis_results.xlsx.

3. Review Results:
Open the generated Excel file to review the sentiment analysis results. Each feedback entry will be accompanied by its sentiment classification, score, and reason.

Notes:
Ensure your dataset has columns for feedback that match the ones specified in the script or update the column names accordingly.
For large datasets, consider optimizing the script for performance.

Author: 
This project is developed and maintained by Priyamvadha Pradeep.
