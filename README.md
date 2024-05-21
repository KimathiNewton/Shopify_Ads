# Shopify Data Extractor and Metrics Calculator
This Python script extracts data and calculates metrics from a Shopify store. It utilizes the Shopify API and Flask web framework.

## Setup:

Replace the placeholder values in the script with your actual Shopify app credentials:
CLIENT_ID
CLIENT_SECRET
REDIRECT_URI (This should match the redirect URI configured in your Shopify app settings)

Run the script:
```
python app.py
```

This will start the Flask development server and listen for requests on http://127.0.0.1:5000/.

## Extracting Data:

Visit http://127.0.0.1:5000/start in your web browser to initiate the OAuth flow for authentication with Shopify.
Follow the on-screen instructions to grant access to your Shopify store.
Upon successful authorization, the script will extract data and calculate metrics for the specified date range (start_date and end_date in the script).
The extracted data with calculated metrics will be saved to a JSON file named data.json.

## Customization:

You can modify the endpoints list in the extract_data function to specify the data you want to fetch from the Shopify API.
The script currently saves the data to a JSON file. You can modify it to integrate with your desired data storage solution.