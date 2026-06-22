# Resume Screening System

An intelligent, automated resume screening system that processes hundreds of resumes against job descriptions and ranks candidates based on skills match, experience, and relevance.

## Features

- **Batch Processing**: Process 500-1000 resumes simultaneously
- **Multi-Format Support**: Parse PDF and DOCX resumes automatically
- **Intelligent Matching**: Weighted scoring algorithm for accurate candidate ranking
- **Skills Taxonomy**: Comprehensive skills database with 1000+ technical and soft skills
- **Web Interface**: User-friendly Streamlit UI for easy interaction
- **Export Options**: Download results as CSV, JSON, or bulk ZIP of top resumes
- **Individual Downloads**: Access each candidate's resume directly from results
- **Contact Extraction**: Automatic extraction of names, emails, and phone numbers

## Architecture

```
Resume_Parser_Project/
├── app.py                  # Streamlit web interface
├── main.py                 # CLI-based processing script
├── screen.py               # Screening logic
├── parsers/
│   ├── resume_parser.py    # Resume text extraction (PDF/DOCX)
│   └── jd_parser.py        # Job description parsing
├── extractors/
│   └── keyword_extractor.py # Skills, experience, keyword extraction
├── matcher/
│   └── scorer.py           # Scoring and ranking algorithm
├── data/
│   ├── config.json         # Scoring weights configuration
│   └── skills_taxonomy.json # Skills database
├── input/                  # Input folder for resumes and JD
├── output/                 # Results storage
└── requirements.txt        # Python dependencies
```