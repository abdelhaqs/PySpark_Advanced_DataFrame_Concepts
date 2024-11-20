# Spark Job Execution Guide for Yellow Taxis Daily Partitioning

## Preparation Steps
1. Enter Docker Container
```bash
docker exec -it pyspark-jupyter-container /bin/bash
```

2. Navigate to Working Directory
```bash
cd work/notebooks/spark-jobs/
```
3. Run Spark Submit Command
```bash
  spark-submit spark-write-partitioned-data-lab-01.py \
  --input_path "/home/jovyan/work/notebooks/datasets/parquet/" \
  --output_path "../datasets/parquet"
```
## Expected Outcome

Partitioned data will be generated in ../datasets/parquet/yellow_taxis_daily/
Partitioning based on p_date column
Output in Parquet format
Overwrites existing data in the output path