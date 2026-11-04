# stb-telemetry-analytics
Maintain a Kafka–Flink telemetry platform that processes set-top-box events, stores analytics data in MinIO/S3 and Apache Doris, and supports dashboards, data quality, and monitoring

<img width="1346" height="470" alt="image" src="https://github.com/user-attachments/assets/7a6b2d6a-34a0-4b65-bf8c-1e6de087438f" />

**Generate events:** set-top-box telemetry service generates events and publish events to Kafka.
**Process streams:** Flink validates, deduplicates, normalizes, and aggregates the events.
**Handle bad data:** Route invalid or duplicate records for quarantine and auditing.
**Store data:** Write event data to MinIO/S3 as Parquet and load processed data into Apache Doris.
**Serve and monitor:** Use SQL, APIs, and dashboards to access insights, with Airflow orchestration and Prometheus/Grafana monitoring.
