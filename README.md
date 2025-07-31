Project Overview

GreenGuard is an AI-powered browser extension that detects, analyzes, and verifies corporate environmental claims in real-time. It empowers consumers to make informed sustainable choices by identifying greenwashing tactics and providing verified environmental information at the point of decision-making.

Defense Panel Feedback Implementation

Feedback Received:
- Enhanced NLP Integration: Panel requested implementation of BERT, spaCy, and HuggingFace transformers
- Real-world Application: Demonstration of working environmental claim detection
- Hybrid Detection Approach: Combination of rule-based and machine learning methods
- **Performance Metrics: Clear confidence scoring and risk assessment

Implementation Response:
- BERT Integration: Implemented DistilBERT for environmental claim classification
- spaCy Analysis: Added linguistic analysis and named entity recognition
- HuggingFace Transformers: Integrated sentiment analysis capabilities
- Hybrid System: Combined rule-based detection with ML models
- Metrics Dashboard: Added confidence scores and greenwashing risk assessment

Key Features

Browser Extension Features:
- Real-time Environmental Claim Analysis - Analyze text and website content for greenwashing indicators
- Comprehensive Education Hub - Learn about the 7 sins of greenwashing and authentic sustainability
- Company Verification System - Verify environmental claims from companies
- Community Reporting- Report suspected greenwashing cases
- Usage Statistics** - Track your impact in fighting greenwashing

Enhanced Backend NLP Features:
- Environmental Claim Detection: Identifies environmental statements in text using BERT
- Greenwashing Risk Assessment: Calculates risk scores for potential greenwashing
- Named Entity Recognition: Extracts organizations, percentages, and dates using spaCy
- Sentiment Analysis: Analyzes tone and sentiment of environmental claims using HuggingFace
- Confidence Scoring: Provides confidence levels for detected claims

Technical Implementation:
- BERT Classification: DistilBERT model for environmental claim classification
- spaCy NLP: Advanced linguistic analysis and entity recognition
- HuggingFace Transformers: RoBERTa-based sentiment analysis
- Flask API: RESTful API endpoints for real-time processing
- MongoDB Integration: Database storage for claims and analysis results
- Smart Contracts: Blockchain integration for transparency

System Requirements

Prerequisites:
- Python 3.8 or higher
- MongoDB (local or cloud instance)
- 4GB+ RAM (for NLP models)
- Internet connection (for model downloads)
- Google Chrome browser (for extension)

Supported Platforms:
- Windows 10/11
- macOS 10.15+
- Ubuntu 18.04+

Installation Instructions

Backend API Setup

Step 1: Clone Repository
git clone https://github.com/Islam-19984/Lastyear_Capston_Backup.git
cd greenguard-mvp-backup then cd backend

Step 2: Create Virtual Environment
Windows
python -m venv venv
venv\Scripts\activate

macOS/Linux
python3 -m venv venv
source venv/bin/activate


Step 3: Install Dependencies

pip install -r requirements.txt

Step 4: Download NLP Models
Download spaCy model
python -m spacy download en_core_web_sm

BERT and HuggingFace models will download automatically on first run

Step 5: Environment Configuration
Create a .env file in the project root:
env
MONGODB_URI=mongodb://localhost:27017/greenguard
FLASK_ENV=development
SECRET_KEY=your-secret-key-here

Step 6: Database Setup
Start MongoDB service
Windows: net start MongoDB
macOS: brew services start mongodb-community
Linux: sudo systemctl start mongod

Browser Extension Setup

Step 1: Download the Extension
- Download this repository as a ZIP file or clone it
- Extract the ZIP file to a folder on your computer

Step 2: Enable Developer Mode in Chrome
- Open Google Chrome browser
- Navigate to chrome://extensions in the address bar
- Toggle Developer mode ON (top-right corner)

Step 3: Load the Extension
- Click Load unpacked button
- Navigate to and select the extracted GreenGuard folder which is extension
- The extension should now appear in your extensions list

Step 4: Pin the Extension
- Click the Extensions icon in Chrome toolbar
- Find GreenGuard and click the pin icon
- The GreenGuard icon should now appear in your toolbar

Step 5: Start Using GreenGuard
- Click the GreenGuard icon in your toolbar
- The extension popup will open
- Navigate through the tabs to explore all features

Running the Application

1: Direct Python Execution
python app.py
 
Flask Development Server
export FLASK_APP=app.py
flask run

Expected Output:

Enhanced NLP processor with BERT/spaCy/HuggingFace loaded successfully
NLP Status: spaCy=True, BERT=True, Sentiment=True
Enhanced NLP:  Enabled
spaCy Linguistic Analysis: Active
BERT Classification: Active
Sentiment Analysis: Active
HuggingFace Transformers: Active
Running on http://127.0.0.1:5000

How to Use

Browser Extension Usage:

#### Analyzer Tab:
- Click the Analyzer tab
- Paste environmental claims in the text area
- Click Analyze Claims
- Review the analysis results

Website Analysis:
- Navigate to a company website
- Click the Analyze Current Page button
- Or enter a URL manually
- Review environmental keywords and warnings

Education Tab:
- Click the Learn tab
- Scroll through comprehensive greenwashing education:
  - What is Greenwashing
  - 7 Sins of Greenwashing
  - SMART Criteria for authentic claims
  - Real-world case studies
  - Tools and resources
  - Action steps

Verification Tab:
- Click the Verify tab
- Enter company name and environmental claim
- Click Verify Claim
- Review verification results

Reporting Tab:
- Click the Report tab
- Select report type
- Enter company name and description
- Submit report

Troubleshooting

Common Issues:

Issue 1: MongoDB Connection Errors
Check MongoDB status
Windows: sc query MongoDB
macOS: brew services list | grep mongodb
Linux: systemctl status mongod


Issue 2: Memory Issues
- Reduce batch size in enhanced_nlp_processor.py
- Use CPU-only PyTorch installation for lower memory usage
- Ensure 4GB+ RAM available

Issue 3: Port Already in Use
bash
Change port in app.py
app.run(host='0.0.0.0', port=5001, debug=True)


Issue 4: Extension Not Loading
- Ensure Developer mode is enabled in Chrome
- Check that you're selecting the correct `extension` folder
- Refresh the extensions page after loading


Model Performance:
- BERT Classification: F1-Score 0.82
- **spaCy NER: 95%+ entity recognition accuracy
- **Sentiment Analysis**: 88%+ sentiment classification accuracy

Recommendations

For Users:
- Use GreenGuard before making eco-conscious purchasing decisions
- Report suspected greenwashing to build community database
- Share educational content to raise awareness
- Leverage the comprehensive company sustainability database

For Developers:
- Test the API endpoints before integrating
- Monitor system resources when running NLP models
- Use the test script to verify functionality

Contributing

Development Setup:
1. Fork the repository
2. Create feature branch: git checkout -b feature-name
3. Make your changes
4. Submit pull request

License

This project is developed as part of an academic capstone project. All rights reserved.

Support

For technical support or questions:
- Email: islamomar2095@gmail.com
- GitHub Issues: Create an issue in this repository
- Video Demo: https://youtu.be/xPr6uuZw5es

Links

- GitHub Repository: https://github.com/Islam-19984/Lastyear_Capston_Backup.git


Join the fight against greenwashing with GreenGuard!

Every verified claim and reported case helps build a more transparent, sustainable future.

Note: This system was developed and tested in response to feedback from the capstone defense panel, incorporating advanced NLP techniques for environmental claim verification.
 