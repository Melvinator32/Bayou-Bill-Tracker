# Bayou Bill Shop Data Tracker

A single-file shop analytics dashboard: revenue and profit trend, advertising
performance, top products, traffic sources, fulfillment status and recent orders,
rendered as hand-built SVG charts with no dependencies and no build step.

## Run it
Open `index.html` in any browser, or serve the folder:

    python3 -m http.server 8000

then visit http://localhost:8000

## Louisiana sales tax monthly report
The **Louisiana Sales Tax — Monthly Report** card at the bottom of the page
builds a return worksheet for any month:

1. In Etsy, open **Shop Manager → Settings → Options → Download Data**, choose
   **Orders**, and download the CSV for the month(s) you need.
2. Click **Import Etsy CSV** and select one or more files. Duplicate orders are
   merged. The file is read in your browser and never uploaded.
3. Pick the month and enter your parish rate. The state rate defaults to 5%.
4. Click **Download CSV** to save the worksheet with its order detail, or
   **Print / Save PDF** to print only the report.

The worksheet splits sales into out-of-state sales, Louisiana sales where Etsy
collected and remitted tax as a marketplace facilitator, and Louisiana sales
with no tax collected. It estimates state and parish tax only on that last
group. It helps you prepare your returns but is not tax advice.

## Demo data
Every figure in this app is invented — product names, order IDs, revenue, ad
spend and traffic counts are all illustrative. There is no live Etsy or Printify
connection and no real shop data is used anywhere.

## Deployment
Pushing to `main` rebuilds the demo at
https://jamesmcknight.me/demos/bayou-bill-shop-tracker/ — see
`.github/workflows/notify-portfolio.yml`.
