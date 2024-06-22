# EchoDetect.ai

## Theme : Fraud Detection and Prevention
## Problem Statement
Develop AI-powered solutions to enhance the integrity of product ratings and reviews, 
and to strengthen counterfeit detection throughout the product lifecycle on the Amazon platform. The 
overarching objective will be to develop innovative AI-driven solutions that can improve the integrity and 
trustworthiness of the Amazon platform, safeguarding both customers and legitimate sellers from fraudulent 
activities. The key elements of the problem statement area) Leveraging language AI and large language 
models (LLMs) to detect fraudulent or suspicious product ratings and reviews on Amazon. The goal will be to 
build applications that can analyze sentiment, identify patterns, and ultimately protect the trust of Amazon's 
customers in the e-commerce ecosystem b) Enhancing Amazon's existing counterfeit detection capabilities by 
leveraging AI across the complete product lifecycle - from the listing of products to the processing of customer 
returns. The aim will be to further strengthen Amazon's ability to prevent counterfeit products from ever entering 
their store.

## Description
Our solution leverages advanced language AI and large language models (LLMs) to detect fraudulent or suspicious product ratings and reviews on Amazon, aiming to analyze sentiment, identify patterns, and protect customer trust. We create interactive dashboards for sellers to gain insights into product performance, pricing, durability, sensitivity, and customer sentiment. Additionally, we automate counterfeit detection throughout the product lifecycle using advanced image and video analysis, significantly reducing manual input. By scrutinizing product images and videos uploaded by sellers, our AI models ensure counterfeit items are detected and rejected before listing. During the return process, our solution analyzes images, videos, and product information to verify the authenticity of returned products, preventing counterfeit items from re-entering the market. This comprehensive approach enhances the integrity and reliability of the Amazon marketplace.

## Block-Diagrams

Seller Dashboard

<img src="https://github.com/mitali-dxt/EchoDetect.ai/assets/131600078/ccc42686-7dac-4e96-ad8f-a3497b3408c9" width="700" height="450">


Amazon Product Upload and Verification

<img src="https://github.com/mitali-dxt/EchoDetect.ai/assets/131600078/0b3ac674-3b69-4551-ad91-6631010ff19d" width="500" height="550">

## Tech Stack
- **React Js**: Frontend Development Framework
- **Node Js, Express Js, Flask, FastApi**: Backend Development Framework
- **Database**: AWS DynamoDB, AWS RDS
- **OpenCV**: YOLO(You Look Only Once)
- **Web Scraping**: Beautiful Soup
- **AI/ML and LLMs**: DeBERTa v3 Large, LDA (Latent Dirichlet Allocation), NMF (Non-negative Matrix Factorization), RAKE (Rapid Automatic Keyword Extraction), TF-IDF (Term Frequency-Inverse Document Frequency), VADER (Valence Aware Dictionary and Sentiment Reasoner), RoBERTa Pretrained LLM Model, KMeans Clustering and Anomaly Detection

## Project Features

### Fake Reviews and Ratings Detection:

1. **"Fake or Genuine" Button:** Integrates a button under each product to analyze reviews and ratings, providing customers with feedback authenticity.

2. **Filtering Fake Reviews:** Filters out fake reviews before generating product summaries, ensuring reliable and trustworthy information for customers.

3. **Genuine Review Analysis:** Uses the DeBERTa v3 large LLM Model to evaluate key aspects such as performance, durability, pricing, and sensitivity, presented in horizontal bar graphs.

4. **Keyword Extraction:**: Displays the most impactful and frequently occurring keywords from genuine reviews, offering quick insights into common themes and concerns.

5. **Image and Video Analysis in Reviews:** Analyzes images and videos in reviews to ensure they match the product, highlighting key observations and visual evidence.
6.  **Personal Assistant Chatbot**: A chatbot powered by Mistral for seamless user support, providing assistance and answering queries in real time.

### Counterfeit Product Detection:

1. **Early Detection during Product Listing:** Uses the YOLO model to analyze product images and videos uploaded by sellers, detecting and rejecting counterfeit items before listing.

2. **Ongoing Monitoring while Products are Listed:** Continuously monitors listed products using AI models to detect any updates or changes indicating counterfeit activity.

3. **Scrutiny during the Product Return Process:** Prompts customers to upload images and videos during return requests, using AI to verify the product’s original condition and prevent fraudulent returns. Generates detailed reports for flagged returns to assist Amazon’s enforcement team.

## Future Scope for Improvement

1. **Amazon Ad Extension:** Develop an extension to detect fake reviews and counterfeit products from Amazon advertisements, enhancing user trust and convenience.

2. **Voice-to-Voice RAG Document Chat:** Implement voice-to-voice RAG Document chat and AI assistant for flexible product analysis and accessibility.

3. **Advanced Review Filtering:** Enable review filtering based on purchase verification and reviewer demographics for personalized insights.

4. **Reward System for Reviewers:** Introduce a reward system for verified reviewers to incentivize honest feedback and enhance review authenticity.

5. **Social Media Expansion:** Expand detection capabilities to identify fake reviews and counterfeit products across social media platforms.

6. **Live Monitoring Dashboards:** Create real-time dashboards for Amazon administrators to monitor and address counterfeit products and fake reviews promptly.


## Installation Steps

### Frontend
1. Rename all `.env.sample` files to `.env` and fill in the required data.
2. Install dependencies: `npm install`
3. Start the development server: `npm run dev`
 
### Backend
1. Navigate to the server directory: `cd server`
2. Install dependencies: `npm install`
3. Start the development server: `npm start`

### Flask Server
1. Set up a conda environment with Python 3.10.
2. Navigate to the chatbot directory: `cd botserver`
3. Install dependencies: `pip install -r requirements.txt`
4. Run the Flask app: `python app.py`






