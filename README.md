# Google BigQuery
As an example, we are going to use the <a href="https://console.cloud.google.com/bigquery?project=bigquery-public-data&page=project">bigquery-public-data Dataset </a>to run a query.


```bash
SELECT faa_identifier, name, longitude, latitude, airport_type, service_city, country
FROM `bigquery-public-data.faa.us_airports`
WHERE airport_use = 'Public'
```

Original package has been extracted from pandas and needs a separate install.

👉 <a href="https://pandas-gbq.readthedocs.io/en/latest/">Documentation</a>

Create (or select) a project in the Google Cloud Console. You need a project_id.

For a private BigQuery table, you will need <a href="https://pandas-gbq.readthedocs.io/en/stable/howto/authentication.html">credentials</a> setup

