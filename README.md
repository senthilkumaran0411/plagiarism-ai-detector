# True-Source

## Overview

**True-Source** is a sophisticated platform designed to help educators and institutions assess the originality of student assignments. The application performs comprehensive plagiarism checks by comparing submitted texts against a vast array of online sources and detecting both direct copying and paraphrasing. It also identifies AI-generated content, ensuring academic integrity and originality.

![image](https://github.com/senthilkumaran0411/plagiarism-ai-detector/blob/a33ecd0e1b75f9bfe60b43538d893bf17665432f/templates/Screenshot%202025-07-30%20221932.png)

## Key Features

| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Plagiarism Detection** | Identifies exact matches and paraphrased content by comparing with online sources |
| **AI Content Detection** | Flags potentially AI-generated text to distinguish from human-written work  |
| **Comprehensive Search** | Uses Google CSE for broad comparison against web content                    |
| **User-Friendly UI**     | Intuitive interface for both students and educators                         |
| **Detailed Reporting**   | Generates reports with copied sections, sources, and similarity percentages |

## Installation Guide

### Prerequisites

- Python 3.x
- Google CSE API Key and Search Engine ID

### Step-by-Step Setup

```bash
# 1. Clone the repository
git clone https://github.com/senthilkumaran0411/plagiarism-ai-detector.git

# 2. Navigate to project directory
cd True-Source

# 3. Install dependencies
pip install -r requirements.txt

4. **Configure Google CSE:**
    - Create a Google CSE and obtain your **API Key** and **Search Engine ID**.
    - Add the credentials to a `.env` file in the following format:
        ```
        {
          "api_key": "YOUR_API_KEY",
          "search_engine_id": "YOUR_SEARCH_ENGINE_ID"
        }
        ```

---

## Usage

To launch the platform or process PDF documents, use:

python main.py
python pdf.py
