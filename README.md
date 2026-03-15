
# NLP-Based Insights from Unstructured Data

## Project Summary
An end-to-end NLP pipeline that retrieves and summarizes insights from 
Yelp reviews using semantic embeddings (Sentence Transformers + FAISS) 
and abstractive summarization (BART / T5).

## Tech Stack
- sentence-transformers (all-MiniLM-L6-v2)
- FAISS (vector similarity search)
- BART / T5 (abstractive summarization)
- Hugging Face Datasets (Yelp reviews)
- pandas, matplotlib, scikit-learn

## How to Run
1. Open the notebook in Google Colab
2. Run Cell 1 (installs) then Runtime > Restart session and run all
3. Query the system using summarize_top_k("your query here")

## How a Team Would Use This
A Customer Success Manager opens the dashboard and types:
'What are customers complaining about this week?'
The system retrieves the 10 most relevant recent reviews and returns 
a 2-sentence summary — no manual reading required.

A Product Manager runs 5 standard queries every Monday morning and 
uses the summaries to prepare talking points for the weekly standup.

## Evaluation Results
See evaluation_results.csv and evaluation_chart.png for human 
usefulness scores across Relevance, Clarity, and Actionability.

## Deployment Vision
- Streamlit dashboard for real-time querying
- Nightly batch summaries emailed to stakeholders
- Slack bot integration for on-demand queries
