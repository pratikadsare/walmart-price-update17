
Walmart Price Update Tool (Bulk + Status from Google Sheet) - v5

Google Sheet headers (fixed):
- SKU
- Publish Status
- Price

Behavior:
- Paste SKU + New Price
- Click "Refresh Status" to auto-fill Publish Status + Current Price
- Hard Fail if any:
  - Blank SKU
  - New Price invalid (blank/not number/<=0)
  - Duplicate SKU
  - SKU Not Found on Walmart
- Download fills template from row 7:
  Column D = SKU
  Columns E,F,G = New Price

Setup:
1) Put template at: templates/walmart_price_template.xlsx
2) pip install -r requirements.txt
3) streamlit run app.py

Important:
- Google Sheet must be shared as: Anyone with the link -> Viewer
