PDFMotor is a cloud-based JSON to PDF rendering API.

<img width="384" height="256" alt="pdfmotor" src="https://github.com/user-attachments/assets/7707c374-4176-4159-9cb7-85e568658d34" />

PDFs are generated synchronously and streamed directly to the client.  
No documents, payloads, or personal data are stored on the server.  
Authentication is handled via API keys.

### Contact 

Website: https://pdfmotor.net  
Contact: info@pdfmotor.net


### Demo API key

Generate a free demo API key instantly on the website.  
Demo keys do not expire and are limited in usage.

### Simple render request

```bash
curl -X POST https://sandbox.pdfmotor.net/v1/render \
  -H "Content-Type: application/json" \
  -H "X-API-Key: YOUR_DEMO_KEY" \
  -d '{
    "title": "Demo PDF",
    "subtitle": "Generated via PDF Motor",
    "fields": [
      { "label": "Name", "value": "John Doe" },
      { "label": "Email", "value": "john@example.com" }
    ]
  }' \
  -o document.pdf

