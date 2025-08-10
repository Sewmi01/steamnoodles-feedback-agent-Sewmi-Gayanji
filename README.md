Name : Sewmi Gayanji
University: NSBM Green University 
Year : 2nd year

#Project Summary – Automated Restaurant Feedback (SteamNoodles)

This project aims to build a multi-agent AI system to automate and enhance restaurant feedback processing for SteamNoodles using LangChain or LlamaIndex.

Agents & Functions

Customer Feedback Response Agent

Input: Single customer review text.

Task: Detect sentiment (positive, negative, neutral) using an LLM.

Output: Generate a short, polite, and context-aware automated reply.

Sentiment Visualization Agent

Input: Date range (e.g., “last 7 days” or custom range).

Task: Create a bar/line plot showing daily counts of positive, negative, and neutral reviews.

Output: Visualization generated dynamically based on review data and user query.

Tools & Technologies

Framework: LangChain or LlamaIndex for agent orchestration.

LLM: OpenAI GPT or HuggingFace Transformers for text analysis and response generation.

Data: Restaurant reviews dataset (text, sentiment, timestamp) from Kaggle.

Visualization: matplotlib, seaborn, or plotly.

Platform: Implemented as a Python script or Jupyter Notebook.

Outcome

Automated, AI-powered customer engagement.

Real-time sentiment analysis and personalized feedback replies.

Interactive sentiment trend visualization for business insights.

 #Testing Instructions
1. Testing the Customer Feedback Response Agent
Goal: Verify that the agent detects sentiment correctly and generates polite, context-aware replies.

Steps:

Prepare Sample Inputs

Create a list of sample feedback covering all sentiment types:

Positive: "The noodles were amazing! I’ll definitely come again."

Negative: "The food was cold and service was slow."

Neutral: "The restaurant is located near the city center."

Run the Agent

Pass each feedback text to the Feedback Response Agent.

Check Outputs

Ensure the sentiment classification matches the actual tone of the text.

Verify that the generated response is:

Polite.

Short (1–3 sentences).

Relevant to the feedback’s content and sentiment.

Edge Case Testing

Mixed sentiment feedback: "The food was good, but the service could be better."

Very short feedback: "Okay."

Extremely long feedback (multiple paragraphs).

Expected Results:

Accurate sentiment label.

Correctly tailored reply (e.g., apology for negative, gratitude for positive).

2. Testing the Sentiment Visualization Agent
Goal: Verify that the agent correctly generates visual sentiment trends for a given date range.

Steps:

Prepare Dataset

Use the Kaggle dataset or your own CSV with review_text, sentiment, and timestamp.

Ensure there are multiple reviews for several different dates.

Run the Agent

Input different date ranges:

"Last 7 days"

"June 1 to June 15"

"Last month"

Check Outputs

A bar or line plot should appear, showing:

X-axis: Dates in the range.

Y-axis: Count of reviews.

Different colors for positive, negative, neutral.

Test Dynamic Filtering

Change the date range and verify that the plot updates accordingly.

Edge Case Testing

Date range with no reviews (should return empty plot or “No data available” message).

Date range with only one sentiment type (plot should still render).

Expected Results:

Correct counts for each sentiment type per day.

Clear, readable plots that change when input changes.

