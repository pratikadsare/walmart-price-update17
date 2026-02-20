
Walmart Price Update Tool (Bulk + Status from Google Sheet) - v6

- Auto-fills Publish Status + Current Price from Google Sheet headers:
  SKU, Publish Status, Price
- Hard Fail (always blocks download):
  blank SKU, invalid price, duplicates, SKU Not Found
- Unpublished SKU:
  shows list in sidebar and requires confirmation checkbox before download
  if confirmed, unpublished SKUs are included in output
- Quick info shows only counts/status, no lists.

Setup:
1) Put template at: templates/walmart_price_template.xlsx
2) pip install -r requirements.txt
3) streamlit run app.py

Sheet must be shared as: Anyone with the link -> Viewer
