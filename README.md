# Yfinance to Snowflake

Daily ETL that downloads one trading session of Yahoo Finance bars and upserts that date into Snowflake (`dev.raw_data.stock_data`).

The DAG lives in `yfinance_to_snowflake.py` (`YfinanceToSnowflake`, 02:30). Default symbol is `MO`. Uses the `snowflake_conn` connection. Designed for Cloud Composer with `apache-airflow-providers-snowflake`.
