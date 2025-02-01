# 📊 Dagster-DLT-DBT Project

## 🚀 Overview
This project integrates **Dagster**, **DLT**, and **DBT** to create a robust data pipeline for efficient data processing, transformation, and analytics.

## ⚙️ Key Features
- **Dagster**: Orchestrates workflows with ease.
- **DLT (Data Load Tool)**: Handles data extraction and loading efficiently.
- **DBT (Data Build Tool)**: Manages data transformation in a modular and scalable way.

## 📂 Project Structure
```
Dagster-DLT/
├── dagster_env/          # Python environment for Dagster
├── dev.duckdb/           # DuckDB database files
├── logs/                 # Log files
├── dbt/                  # DBT project folder
├── pyproject.toml        # Project dependencies and configuration
└── setup.py              # Project setup script
```

## 🚀 Getting Started
### 1️⃣ Prerequisites
- Python 3.8+
- Docker (optional, for containerized deployments)
- Git

### 2️⃣ Installation
```bash
git clone <repository-url>
cd Dagster-DLT-DBT
python -m venv dagster_env
source dagster_env/bin/activate  # For Unix
# OR
.\dagster_env\Scripts\activate   # For Windows
pip install -r requirements.txt
```

### 3️⃣ Running the Project
```bash
dagster dev  # Start the Dagster development server
dbt run       # Execute DBT models
dlt load      # Run DLT data load tasks
```

## 🗂️ Configuration
Ensure the following files are correctly configured:
- **`.env`**: Store environment variables.
- **`profiles.yml`** (DBT): DBT connection profiles.
- **Dagster Settings**: Located in `dagster.yaml`.

## 📝 Usage
- **Dagster UI:** Navigate to [localhost:3000](http://localhost:3000) to access the Dagster UI.
- **DBT Models:** Modify `.sql` files in the `dbt/models` directory.
- **DLT Pipelines:** Define pipelines in the `dlt/` folder.

## 🐞 Troubleshooting
- **Common Errors:**
  - `DagsterUserCodeUnreachableError`: Ensure the Dagster user code server is running.
  - Database connection issues: Verify credentials in `profiles.yml`.

## 🤝 Contributing
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## 📜 License
This project is licensed under the MIT License.

## 🙌 Acknowledgements
- [Dagster](https://dagster.io/)
- [DLT](https://dlt.dev/)
- [DBT](https://www.getdbt.com/)

---

*Happy Data Engineering! 🚀📊*

