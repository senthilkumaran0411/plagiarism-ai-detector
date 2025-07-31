# 🔍 True-Source: Plagiarism & AI Content Detection Platform

## Overview

**True-Source** is a sophisticated platform designed to help educators and institutions assess the originality of student assignments. The application performs comprehensive plagiarism checks by comparing submitted texts against a vast array of online sources and detecting both direct copying and paraphrasing. It also identifies AI-generated content, ensuring academic integrity and originality.

---

![True-Source Screenshot](https://github.com/senthilkumaran0411/plagiarism-ai-detector/blob/a33ecd0e1b75f9bfe60b43538d893bf17665432f/templates/Screenshot%202025-07-30%20221932.png)

---

## 🚀 Key Features

| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Plagiarism Detection** | Identifies exact matches and paraphrased content by comparing with online sources |
| **AI Content Detection** | Flags potentially AI-generated text to distinguish from human-written work  |
| **Comprehensive Search** | Uses Google CSE for broad comparison against web content                    |
| **User-Friendly UI**     | Intuitive interface for both students and educators                         |
| **Detailed Reporting**   | Generates reports with copied sections, sources, and similarity percentages |

---

## 🗂️ Project Structure

```
True-Source/
├── main.py                   # Main application entry point
├── pdf.py                    # PDF document processing
├── requirements.txt          # Python dependencies
├── .env                      # Environment configuration file
│
├── templates/
│   ├── index.html           # Main interface
│   ├── results.html         # Results display page
│   └── upload.html          # File upload page
│
├── static/
│   ├── css/
│   │   └── style.css        # Application styles
│   └── js/
│       └── script.js        # Frontend functionality
│
└── uploads/                 # Temporary file storage
```

---

## ⚙️ Installation Guide

### Prerequisites

- Python 3.x
- Google CSE API Key and Search Engine ID

### Step-by-Step Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/senthilkumaran0411/plagiarism-ai-detector.git
   ```

2. **Navigate to project directory:**
   ```bash
   cd True-Source
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Google CSE:**
   - Create a Google CSE and obtain your **API Key** and **Search Engine ID**.
   - Add the credentials to a `.env` file in the following format:
     ```json
     {
       "api_key": "YOUR_API_KEY",
       "search_engine_id": "YOUR_SEARCH_ENGINE_ID"
     }
     ```

---

## 📋 Usage

### Launch the Platform

To launch the main platform:
```bash
python main.py
```

### Process PDF Documents

To process PDF documents specifically:
```bash
python pdf.py
```

### Web Interface

1. Open your browser and navigate to `http://localhost:5000`
2. Upload your document or paste text directly
3. Click "Check for Plagiarism" to analyze the content
4. Review the detailed report with highlighted matches and sources

---

## 🔧 Configuration

### Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
GOOGLE_API_KEY=your_google_cse_api_key
SEARCH_ENGINE_ID=your_search_engine_id
FLASK_ENV=development
FLASK_DEBUG=True
```

### Supported File Formats

- **Text Files**: `.txt`, `.docx`
- **PDF Files**: `.pdf`
- **Direct Text Input**: Copy and paste functionality

---

## 📊 Features in Detail

### Plagiarism Detection
- **Exact Match Detection**: Identifies word-for-word copying
- **Paraphrase Detection**: Recognizes rewritten content with similar meaning
- **Source Attribution**: Provides links to original sources
- **Similarity Scoring**: Percentage-based similarity metrics

### AI Content Detection
- **Machine Learning Models**: Advanced algorithms to detect AI-generated text
- **Confidence Scoring**: Probability scores for AI-generated content
- **Pattern Recognition**: Identifies common AI writing patterns

### Reporting System
- **Visual Highlights**: Color-coded text showing plagiarized sections
- **Source Links**: Direct links to matching online content
- **Downloadable Reports**: PDF export functionality
- **Similarity Statistics**: Comprehensive analysis metrics

---

## 🔍 API Integration

### Google Custom Search Engine (CSE)

True-Source leverages Google CSE to perform comprehensive web searches:

```python
# Example API usage
import requests

def search_content(query, api_key, search_engine_id):
    url = f"https://www.googleapis.com/customsearch/v1"
    params = {
        'key': api_key,
        'cx': search_engine_id,
        'q': query
    }
    response = requests.get(url, params=params)
    return response.json()
```

---

## 🛠️ Dependencies

```txt
Flask==2.3.3
requests==2.31.0
python-docx==0.8.11
PyPDF2==3.0.1
beautifulsoup4==4.12.2
nltk==3.8.1
scikit-learn==1.3.0
numpy==1.24.3
pandas==2.0.3
python-dotenv==1.0.0
```

---

## 🚨 Important Notes

### Academic Use Only
This tool is designed for educational purposes to promote academic integrity. Users should:
- Respect copyright and intellectual property rights
- Use the tool ethically and responsibly
- Understand institutional policies on plagiarism detection

### API Limitations
- Google CSE has daily query limits
- Large documents may require processing time
- Internet connection required for online source comparison

---

## 🤝 Contributing

We welcome contributions to improve True-Source! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature-name`
3. **Commit your changes**: `git commit -m 'Add feature'`
4. **Push to the branch**: `git push origin feature-name`
5. **Submit a pull request**

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Thank You!

<div align="center">
  
  ![Typing Animation](https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=2000&pause=500&color=22D3EE&width=500&lines=Thank+You+for+Using+True-Source!;Promoting+Academic+Integrity+📚)
  
  <br>
  
  <img src="https://raw.githubusercontent.com/senthilkumaran0411/plagiarism-ai-detector/main/assets/true-source-logo.gif" width="150" alt="True-Source Logo">
  
  <br><br>
  
  **Contact Us:**
  
  📧 **Email:** [senthilkumaran0411@gmail.com](mailto:senthilkumaran0411@gmail.com)  
  💻 **GitHub:** [senthilkumaran0411](https://github.com/senthilkumaran0411)  
  🔗 **LinkedIn:** [Connect with us](https://linkedin.com/in/senthilkumaran0411)
  
  <br>
  
  **⭐ If you found this project helpful, please give it a star!**
  
</div>

---

<div align="center">
  
</div>
