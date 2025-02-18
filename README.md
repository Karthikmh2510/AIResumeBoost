# AIResumeBoost

Boost your resume for job applications. This is a Resume Analyzer with an ATS Feedback system.


This repository contains the code for a **Smart ATS Resume Analyzer** built using **Streamlit**, **Google Gemini Models**, and **PyPDF2**. This application helps users improve their resumes based on job descriptions by providing feedback, suggestions, and corrections.

## Features
- **Upload Resume (PDF):** Users can upload their resume in PDF format.
- **Job Description Analysis:** Matches resumes to job descriptions and provides feedback.
- **Resume Improvement Suggestions:** Offers detailed recommendations for resume enhancement.
- **Sentence Corrections:** Corrects specific sections such as objectives, skills, and work experience.
- **Supports Google Gemini Models:** Integrates Gemini 2.0 Flash and Gemini 2.0 Flash Thinking.

## Requirements
- Python 3.9+
- Streamlit
- PyPDF2
- google-generativeai
- python-dotenv

## Installation
```bash
# Clone the repository
git clone https://github.com/Karthikmh2510/AIResumeBoost.git

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
```

## Setup
1. **Google API Key:** Create a `.env` file in the root directory and add your Google API key:
   ```
   GOOGLE_API_KEY=your_google_api_key
   ```

## Usage
```bash
# Run the Streamlit app
streamlit run app.py
```
- **Paste Job Description** and **Upload Resume**.
- Click on any button:
  - **Get Resume Feedback:** Provides ATS score and keyword suggestions.
  - **Suggest me changes:** Gives section-by-section recommendations.
  - **Correct my Resume in detail:** Provides detailed corrections for each resume section.

## File Structure
```
smart-ats-resume-demo/
│── app.py                  # Main Streamlit App
│── .env                    # API Key Configuration
│── requirements.txt        # Python Dependencies
└── README.md               # Project Documentation
```

## Prompts Used
Two structured prompts are used:
- **Prompt 1:** ATS-based feedback and keyword suggestions.
- **Prompt 2:** Resume section improvement with corrected examples.

## Rate Limits
- **Gemini 2.0 Flash:** 15 Requests/min, 1500 Requests/day
- **Gemini 2.0 Flash Thinking Exp:** 10 Requests/min, 1500 Requests/day

## License
This project is licensed under the MIT License.

## Contribution
Contributions are welcome! Please feel free to fix the repository and submit a pull request.

## Contact
For any questions, please contact [karthik.m.hadagali2013@gmail.com](mailto:karthik.m.hadagali2013@gmail.com).

