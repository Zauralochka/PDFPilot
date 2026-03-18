# 🚀 PDF Pilot

**PDF Pilot** is an AI-powered document intelligence system that automates the naming, redaction, classification, and organization of PDF documents across multiple industries.

It transforms unstructured, inconsistent document collections into **standardized, searchable, and compliant digital archives**.

---

## 🧩 Problem

Organizations across industries (government, education, healthcare, corporate) receive **large volumes of documents** daily.

For example, development applications may include:

- Architectural plans  
- Engineering reports  
- Environmental assessments  
- Statutory declarations  

Currently, staff must manually:

- Review documents  
- Rename files according to internal conventions  
- Identify and redact personally identifiable information (PII)  
- Organize documents for publication or storage  

⚠️ This process is:
- Time-consuming  
- Error-prone  
- Difficult to scale  

---

## 💡 Solution

**PDF Pilot** introduces an intelligent, AI-driven workflow that:

- 🏷️ Automatically names documents using domain-specific conventions  
- 🔒 Detects and redacts sensitive information (PII)  
- 🧠 Extracts structured metadata using NLP (NER)  
- 🔍 Finds similar documents for consistent naming  
- 📊 Provides a human-in-the-loop review interface  

---

## 🧠 Core Features

### 📤 Batch Document Processing
Upload and process multiple documents simultaneously.

---

### 🏷️ Domain-Aware Naming Engine
Supports **multiple industries** with configurable naming conventions.

| Domain        | Example Naming Convention                          |
|--------------|--------------------------------------------------|
| Development   | `{Date}_{ProjectName}_{DocumentType}`             |
| Education     | `{StudentName}_{DocumentType}_{Year}`             |
| Healthcare    | `{PatientID}_{DocumentType}_{Date}`               |
| Corporate     | `{Company}_{DocumentType}_{Version}`              |

---

### 🔍 Similarity-Based Naming
Ensures consistency by learning from existing documents.

- Finds semantically similar documents  
- Reuses naming patterns  
- Adapts names based on extracted entities  

---

### 🧠 Metadata Extraction (NER)
Automatically extracts structured data from documents.

#### Example Entities

- **Development** → Address, Application ID, Project Name  
- **Education** → Student Name, Year, School  
- **Healthcare** → Patient ID, Test Type, Date  

#### Example Output

```json
{
  "domain": "development",
  "address": "12 Ocean Street, Bondi NSW",
  "document_type": "Environmental Impact Assessment",
  "date": "2025-02-14"
}
