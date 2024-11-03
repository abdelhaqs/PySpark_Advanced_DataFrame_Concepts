# PySpark Advanced DataFrame Concepts

This project provides a Docker-based setup to explore advanced PySpark DataFrame concepts using Jupyter notebooks. The environment includes all necessary dependencies, making it easy to get started with PySpark for data processing and analysis.

## Project Overview

- **Jupyter Notebooks:** Interactive notebooks to experiment with PySpark code.
- **PySpark:** A Python library for Spark, used for large-scale data processing.
- **Docker:** Containerization tool to ensure a consistent development environment.

## Setup Instructions

Follow these steps to set up and run the project on your local machine.

### 1. Prerequisites

Ensure you have the following installed on your machine:

- [Docker](https://www.docker.com/products/docker-desktop) (for containerized development)
- [Git](https://git-scm.com/downloads) (for cloning the repository)

### 2. Clone the Repository

Clone this GitHub repository to your local machine:

```bash
git clone https://github.com/your_username/PySpark_Advanced_DataFrame_Concepts.git
cd PySpark_Advanced_DataFrame_Concepts


### 3. Download the NYC Taxi Trip Data

This project uses the NYC Taxi Trip Data in Parquet format as an example dataset. You can download the dataset from the [NYC Taxi & Limousine Commission website](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).

#### Download the Parquet file(s):
- Choose the relevant data files in Parquet format.

#### Place the files in the datasets folder:
- After downloading, place the Parquet files in the following directory:

```bash
notebooks/datasets
```

### 4. Build and Run the Docker Container

This project uses the official `jupyter/pyspark-notebook` Docker image. The `docker-compose.yml` file is included for easy setup.

#### Start Docker Compose

1. **Build and run the container using Docker Compose:**

   ```bash
   docker-compose up
   ```

2. **Access Jupyter Lab:**
   - Once the container is running, open your web browser and navigate to [http://localhost:8888](http://localhost:8888). Use the token provided in the terminal to log in.

#### Stop Docker Compose

To stop the running Docker containers, use the following command:

```bash
docker-compose down
```

### 5. Start Exploring

Once the container is running, open Jupyter Lab at [http://localhost:8888](http://localhost:8888) in your web browser. You'll find the notebooks inside the `/home/jovyan/work/notebooks` directory.

### Project Structure

- **/notebooks**: Contains Jupyter notebooks for various PySpark DataFrame operations.
- **/notebooks/datasets**: Directory for datasets used in the notebooks.
- **Dockerfile**: Defines the Docker image for this project (optional if using `jupyter/pyspark-notebook` directly).
- **docker-compose.yml**: Docker Compose file to manage the container setup.
