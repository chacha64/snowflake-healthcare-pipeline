# 🏥 Healthcare Claims Pipeline — Advanced (Pro) (AWS S3 → Snowflake)

This is a production-style Snowflake project that demonstrates:
- Auto-ingestion from AWS S3 with **Snowpipe**
- **Streams & Tasks** for CDC
- **SCD Type 2** handling for the `DIM_PATIENT` table
- Incremental **MERGE** into `FACT_CLAIMS`
- **Data Quality** checks and **Error Logging**

## Structure
```
scripts/
  01_objects.sql
  02_stage_and_pipe.sql
  03_dim_patient_scd2.sql
  04_fact_claims_merge.sql
  05_tasks.sql
  06_validation_and_monitoring.sql
data/
  patients_day1.csv
  patients_day2.csv
  claims_day1.csv
```
> Replace placeholders: `MY_S3_INTEGRATION`, `s3://health-claims-bucket/`, and `COMPUTE_WH`.
