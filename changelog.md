# Record of steps taken

## 1 - Install WSL2

```cmd
# wsl --unregister Ubuntu  # as Ubuntu already existed from a failed install
wsl --install

sudo apt update && sudo apt upgrade
# Updates the local package list and upgrades installed packages to the latest versions.
# Ensures your system is secure, stable, and compatible with newer software.

sudo apt install build-essential
# Installs core development tools: GCC (C/C++ compiler), make, and essential libraries.
# Required for compiling software from source and building Python packages with native extensions.
```

## 2 -Create project directory 

```cmd
sudo apt update
sudo apt install tree

mkdir trino\etc
mkdir trino\catalog
mkdir scripts
mkdir sql
mkdir data\bronze
mkdir data\silver
mkdir data\gold
mkdir data\downloads
mkdir notebooks
mkdir tests
mkdir docs
mkdir logs
mkdir config

tree -F
```

## 3 - Add Project Structure to ReadMe

```
databricks-housing-platform/
├── docker-compose.yml          # Trino container configuration
├── requirements.txt            # Python dependencies
├── README.md                   # This file
├── .gitignore                  # Git ignore rules
├── trino/                      # Trino configuration
│   ├── etc/                    # Trino server config
│   └── catalog/                # Data source connectors
├── sql/                        # SQL scripts
├── scripts/                    # Python ETL scripts
├── notebooks/                  # Jupyter notebooks for analysis
├── data/                       # Data files (gitignored)
│   ├── bronze/
│   ├── silver/
│   └── gold/
└── docs/                       # Documentation
```
