1. Create a project in Google Cloud
2. Connect a Google Sheet to Google BigQuery
3. Create a Service Account
4. Create a JSON key for the Service Account
5. Enable the BigQuery API, Google Sheets API, and Google Drive API
6. Install the gcloud CLI
7. Initialise the gcloud CLI
8. Authenticate the gcloud CLI
9. Install the google-cloud-bigquery library and google-oauth2-service-account library
10. Create a credentials including the service account key and scope. The reason why have to provide a Google Drive API for the scope because the Google Drive loads the data from the Google Sheet and the service account does not have the role that can access to the Google Sheet. However, the service account has the role that can access the Google BigQuery. Another reason is that when the Google Sheet's data is loaded by Google Drive to BigQuery, the data is belonged to Google Cloud. Therefore, have to call the Google Cloud Platform API to grant access to the BigQuery's data, which is the reason why do not have to call the Google BigQuery API.
11. Create a project id
12. Create a BigQuery client
13. Query the BigQuery table
14. Create a dataframe using the query's result
15. Create a function that returns a dictionary containing fundraiser's inputs