# Kountifi-task1-Intelligent-Invoice-Parser(Intermediate AI)

### 🧠 Objective
Simulate intelligent invoice parsing using Python and basic NLP techniques.

### 📝 Instructions
- Read a sample invoice (PDF or text format) using Python.
- Extract key fields from the document:
  - **Invoice Number**
  - **Vendor**
  - **Total**
  - **Date**
  - **Due Date**
  - **Line Items**
- Use `pdfplumber` or `PyMuPDF` to extract text from PDF files.
- Apply regular expressions (`regex`) for field detection.
- (Optional Bonus) Use a **language model** (e.g., OpenAI API or HuggingFace Transformers) to clean and validate the extracted fields.

### ⚙️ Technologies Used
- `pdfplumber` – PDF text extraction
- `re` – Regular expressions for pattern matching
- `transformers` – Zero-shot validation with DistilBERT (HuggingFace)
- `json` – Output formatting
- `uuid` – Artifact tracking
- `tqdm` – Progress bar

### ✅ Expected Output
- A cleaned and structured JSON containing:
  - Extracted invoice fields
  - Line items in a list of dictionaries
  - An auto-generated artifact ID
- A Python script with clear function breakdown and comments
- Console output showing the parsed results

### 📦 Output Example
```json
{
    "invoice_number": "INV-12345",
    "vendor": "Acme Corporation",
    "total": "458.00",
    "date": "01/15/2024",
    "due_date": "01/30/2024",
    "line_items": [
        {
            "quantity": "2",
            "description": "Consulting Services",
            "price": "200.00"
        },
        {
            "quantity": "1",
            "description": "Travel Reimbursement",
            "price": "58.00"
        }
    ],
    "artifact_id": "b4f7d5c4-91e8-4e32-8a27-1ec4efb9fa9b"
}
