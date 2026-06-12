# Intelligent AP Automation: Invoice Processing via Nanonets LLM Agents

An end-to-end Intelligent Document Processing (IDP) project utilizing **Nanonets LLM-powered Agents** to eliminate manual data entry in Accounts Payable. This automation workflow intercepts incoming multi-format invoice files directly through email triggers, extracts highly structured transaction variables (**Invoice Number, Date, Vendor Name, and Total Amount**), and instantly streams the synchronized records into a production Google Sheet tracker.

---

## 🛠️ System Architecture & Workflow Pipeline

The entire document ingestion and structured extraction engine is implemented step-by-step as outlined below:

### 1. Cloud Infrastructure Integration
Connect external systems to the Nanonets environment to safely authorize read/write capabilities across target spreadsheets.
![Google Sheets Integration Setup](images/01_connector_setup.jpg)

### 2. Creating and Prompting the Extract Agent
Configure a standalone LLM agent with plain-English instructions defining the target data nodes to look for on any incoming document layout.
![Nanonets Agent Rule Base Configuration](images/02_agent_setup.png)

### 3. Integrating the Downstream Action Tool
Map the custom-tailored Google Sheets append action as an active workflow tool inside the processing flow.
![Workflow Tool Configuration Map](images/03_tool_integration.png)

### 4. Direct Column-to-Variable Property Mapping
Align extracted data fields cleanly with the matching column tracking schemas defined inside the target spreadsheet file.
![Data Object Schemas Mapping Screen](images/04_variable_mapping.png)

---

## 📊 Live Execution & Verified Production Results

### 5. Automated Email Ingestion Ingress Gateway
The workflow provides a dedicated, unique email address wrapper. Any invoices forwarded to this email address trigger the automation engine immediately.
![Nanonets Email Processing Trigger Endpoint](images/05_email_trigger.png)

### 6. Centralized Monitoring Logs & Audit Trails
Track bulk runs in real-time within the platform's execution interface, logging comprehensive task records alongside runtime statistics.
![Active Processing Queue Interface](images/06_processing_queue.png)

### 7. Real-Time Document Parsing Verification
Validate extraction accuracy directly in the dashboard UI, verifying that visual boundary frames match the parsed text before saving.
![Nanonets Document Extraction Validation UI](images/07_task_validation.png)

### 8. Final Extracted Output in Google Sheets
Once validation transitions to complete, the structured rows populate autonomously into your target spreadsheet tracking ledger.
![Populated Production Spreadsheet Target Logs](images/08_final_sheets_output.png)

---

## ⚙️ Project Reproduction & Setup Summary

1. **Sign Up**: Set up a workspace profile at [Nanonets](https://nanonets.com).
2. **Authorize Connection**: Navigate to `Sidebar -> Connectors` and link your target Google account.
3. **Build the Extraction Agent**: Initialize a new **Extract Agent** using the precise system prompts configured in **Step 2**.
4. **Deploy Global Inbound Email**: Copy your unique agent trigger email path, forward a batch of invoice sample PDFs, and watch data records synchronize instantly inside your cloud tracking file.
