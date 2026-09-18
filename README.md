# Metadata Stripper

A Python-based **metadata anonymization and file privacy tool** that processes supported digital files to remove or modify available metadata, randomize timestamps, and generate anonymized filenames.

The application provides a simple **Tkinter graphical interface** for selecting and processing files.

---

## 🔎 Overview

Digital files can contain metadata that may reveal information about the file, its author, creation history, or other properties.

Metadata Stripper was developed as a cybersecurity and privacy-focused utility to explore how metadata can be identified, removed, modified, and anonymized across different file formats.

The project demonstrates practical experience with:

- File metadata handling
- Data sanitization
- Privacy protection
- Python automation
- GUI application development
- Digital forensics concepts

---

## 🚀 Key Features

- 🧹 **Metadata Processing** — Removes or modifies available metadata in supported file types.
- 🕒 **Timestamp Randomization** — Changes filesystem timestamps on processed output files.
- 🔐 **Metadata Anonymization** — Replaces selected metadata fields with generated random values where supported.
- 🔤 **Filename Randomization** — Generates an anonymized output filename.
- 🖥️ **Graphical Interface** — Provides a simple Tkinter-based interface for selecting files.
- 📁 **Multi-Format Processing** — Supports image, PDF, audio, and Word document processing.

---

## 📂 Supported File Types

### Images

- JPG / JPEG
- PNG
- WebP
- BMP
- TIFF

Image processing includes removal of EXIF metadata and conversion to a selected image format.

### PDF

- PDF

PDF processing modifies document metadata and cleans page contents.

### Audio

The current implementation includes processing support for:

- MP3
- FLAC
- OGG
- Opus
- AAC

> WAV is currently recognized by the file-type detection function but does not yet have a dedicated processing implementation.

### Word Documents

- DOCX

> The current implementation uses `python-docx`, so DOCX is the supported Microsoft Word format.

### Video

The application recognizes:

- MP4
- MOV
- AVI
- MKV
- WMV
- FLV

> Video files are currently copied and their filesystem timestamps are randomized. Full embedded video metadata removal is not currently implemented.

---

## 🛠️ Technologies Used

- **Python**
- **Tkinter** — Graphical user interface
- **Pillow** — Image processing
- **Piexif** — EXIF metadata handling
- **PyMuPDF (fitz)** — PDF processing
- **Mutagen** — Audio metadata handling
- **python-docx** — DOCX document processing
- **NumPy** — Imported in the project for numerical processing

---

## 🔄 Processing Workflow

```text
                 Select File
                     │
                     ▼
               Detect File Type
                     │
          ┌──────────┼──────────┐
          ▼          ▼          ▼
       Image       PDF       Audio/DOCX
          │          │          │
          └──────────┼──────────┘
                     ▼
             Metadata Processing
                     │
                     ▼
           Timestamp Randomization
                     │
                     ▼
            Filename Randomization
                     │
                     ▼
             Anonymized Output
``` 
---

**Main Files**

metadata.py

The main Python application containing:

- File type detection
- Metadata processing functions
- Timestamp randomization
- Filename randomization
- Tkinter graphical interface

**Tools.md**

Additional documentation related to the tools and functionality used by the project.

**README.md**

Project documentation, installation instructions, features, and usage information.

---

### ⚙️ Installation
1. Clone the Repository
   
git clone https://github.com/Ms-Nasir/Metadata-Stripper.git

2. Navigate to the Project Directory

cd Metadata-Stripper

3. Install Required Dependencies

pip install pillow piexif pymupdf mutagen python-docx numpy

Tkinter is included with most standard Python installations. On some Linux distributions, it may need to be installed separately.

---

### ▶️ Usage

Basic Workflow

1. Launch the application.
2. Click Select File.
3. Choose a supported file.
4. Select the output location.
5. The application processes the file.
6. Metadata processing and timestamp randomization are performed according to the file type.
7. The output file receives an anonymized filename.

--- 

### 🔐 Cybersecurity & Privacy Applications

Metadata Stripper demonstrates practical concepts relevant to:

- Privacy protection
- Data sanitization
- Secure file handling
- Metadata analysis
- Digital forensics
- Information exposure
- Cybersecurity tool development

Metadata can contain contextual information that may be relevant during security and forensic investigations. Understanding how metadata is created, modified, and removed is therefore useful for both privacy protection and digital forensics.

---

### 🎯 Project Objectives

The main objectives of this project are to:

- Explore metadata and its privacy implications.
- Develop a Python-based metadata processing utility.
- Automate metadata modification for supported file formats.
- Implement timestamp and filename anonymization.
- Provide a simple graphical interface for users.
- Strengthen practical Python and cybersecurity skills.

---

### 🔮 Potential Enhancements

Future improvements may include:

- Full embedded metadata removal for supported video formats.
- WAV metadata processing.
- Additional document formats.
- Batch file processing.
- Before-and-after metadata comparison.
- Detailed metadata removal reports.
- Improved error handling and user feedback.
- Expanded metadata inspection capabilities.

---

### 📚 Learning Outcomes

This project provided practical experience with:

- Python application development
-File processing
- Metadata manipulation
- EXIF handling
- PDF metadata processing
- Audio metadata processing
- DOCX document processing
- Timestamp manipulation
- GUI development using Tkinter
- Privacy and data-sanitization concepts
- Digital forensics fundamentals

---


### 👩‍💻 Author

Ms. Nasir

Cybersecurity | SOC Operations | Network Security | Digital Forensics
