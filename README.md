# fuel-prices-elt
Daily ELT pipeline on French fuel prices open data with dlt, BigQuery, dbt, Github Actions

Project status : work in progress ...

The objective is to build a production-like data pipeline that answers 3 majors questions in an energy crisis period:
    - How do fuel prices evolve over time, especially, especially by fuel type and French region ?
    - What is the breakdown of open and closed stations by region ?
    - Is there a price gap between motorway and non-motorway gas stations ?


stack :
    - Ingestion : dlt (Python)
    - Storage : BigQuery
    - Transformation : dbt (SQL, Jinja)
    - Data Quality : dbt tests
    - Scheduling : GitHub Actions (cron)
    - CI : GitHub Actions


sources : 
    - https://www.prix-carburants.gouv.fr/rubrique/opendata/
