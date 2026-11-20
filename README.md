# 🌅 TEXT to JSON Converter (Anime Twilight Edition)

A structured data extraction web app built with **Streamlit**, **`google-genai` (`gemini-3.5-flash-lite`)**, **Pydantic**, and **Pandas** that turns unstructured text and files into strict, valid JSON with an Anime Twilight UI.

## ✨ Key Features

* **AI Auto-Schema Discovery & Dynamic Pydantic Validation:** Automatically infers context-relevant JSON keys from raw text, compiles a Pydantic model on the fly, and enforces structured output via `response_mime_type="application/json"` and `response_schema`, backed by a regex JSON sanitizer.
* **Instant Auto-Convert on Paste / Upload:** Converts pasted or typed text automatically (toggleable), with a manual **Convert to JSON →** trigger when preferred.
* **Multi-File Batch Processing:** Upload multiple `.txt`, `.md`, `.csv`, or `.log` files at once and export a combined JSON array.
* **Data Quality Completeness Score:** Evaluates the proportion of populated fields in single-record extractions and flags incomplete outputs.
* **Prompt Injection Guardrail Test Suite:** Includes a one-click jailbreak test payload and XML-delimited system instructions (`<raw_input>`) designed to treat untrusted text as inert data.
* **Multi-Format Exports:** Download results as **JSON**, **CSV**, or **Excel (`.xlsx`)**.
* **Anime Twilight UI:** Styled with deep twilight navy/slate cards, sunset amber-to-orange accents, and responsive layout controls.

## 🛠️ Tech Stack

* **Frontend / App Framework:** Streamlit
* **LLM & Structured Outputs:** `google-genai` (`gemini-3.5-flash-lite`)
* **Schema Enforcement:** Pydantic (`create_model`, `Field`)
* **Data & Exports:** Pandas, `openpyxl`

## 🚀 Local Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Vaibhav11-tech/text-to-json-converter.git](https://github.com/Vaibhav11-tech/text-to-json-converter.git)
   cd text-to-json-converter
