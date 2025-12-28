# ADGM-Compliant Corporate Agent

An intelligent AI-powered legal assistant that reviews, validates, and helps users prepare documentation for business incorporation and compliance within the Abu Dhabi Global Market (ADGM) jurisdiction.

## Features

- Document Upload & Analysis: Accept .docx documents and identify their types
- Compliance Checking: Verify completeness based on ADGM rules
- Red Flag Detection: Highlight legal issues and inconsistencies
- Document Annotation: Insert contextual comments in documents
- Missing Document Identification: Check for required documents based on process type
- Structured Reports: Generate JSON reports of findings

## Setup Instructions

1. Clone this repository:
```
git clone <repository-url>
cd adgm-corporate-agent
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Run the application:
```
streamlit run app.py
```

## Usage

1. Upload one or more .docx documents related to ADGM processes
2. The system will:
   - Identify document types
   - Determine the process you're attempting (incorporation, licensing, etc.)
   - Check for missing required documents
   - Review documents for compliance issues
   - Insert comments in documents where issues are found
   - Generate a structured report of all findings
3. Download the annotated documents and JSON report

## Document Categories Supported

1. **Company Formation Documents**
   - Articles of Association (AoA)
   - Memorandum of Association (MoA/MoU)
   - Board Resolution Templates
   - Shareholder Resolution Templates
   - Incorporation Application Form
   - UBO Declaration Form
   - Register of Members and Directors
   - Change of Registered Address Notice

2. **Licensing Regulatory Filings**

3. **Employment HR Contracts**

4. **Commercial Agreements**

5. **Compliance Risk Policies**

## Architecture

- **Frontend**: Streamlit web interface
- **Document Processing**: python-docx library
- **Text Analysis**: Regular expression pattern matching
- **Output**: Annotated .docx files and structured JSON reports
