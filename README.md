# Bayou Bill Shop Data Tracker

A single-file shop analytics dashboard: revenue and profit trend, advertising
performance, top products, traffic sources, fulfillment status and recent orders,
rendered as hand-built SVG charts with no dependencies and no build step.

## Run it
Open `index.html` in any browser, or serve the folder:

    python3 -m http.server 8000

then visit http://localhost:8000

## Demo data
Every figure in this app is invented — product names, order IDs, revenue, ad
spend and traffic counts are all illustrative. There is no live Etsy or Printify
connection and no real shop data is used anywhere.

## Deployment
Pushing to `main` rebuilds the demo at
https://jamesmcknight.me/demos/bayou-bill-shop-tracker/ — see
`.github/workflows/notify-portfolio.yml`.
