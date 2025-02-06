# Journal Archive Tool

A tool to efficiently archive, store, and query logs (journal files).

---

## 📋 Table of Contents
- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🚀 Features
- **Log Collection**: Collects logs from files or streams.
- **Log Storage**: Archives logs in an SQLite database.
- **Log Querying**: Allows searching and viewing archived logs.
- **Log Management**: Automatically deletes old logs to save space.

---

## 📥 Installation

### Prerequisites
- Python 3.x
- pip (Python package manager)

### Steps
1. Clone the repository:
2. 
   ```bash
   git clone https://github.com/m-brakni/journal-archive-tool.git

## Navigate to the project directory:
cd journal-archive-tool

## Install the dependencies:
 ```bash
pip install -r requirements.txt

🛠 Usage
Collect and Store Logs

    Place your log files in the project directory (e.g., app.log).

    Run the main script:

```bash
python src/main.py --collect

Logs will be collected and stored in the database.

## Query Logs
To search for logs containing a specific keyword:
```bash
python src/main.py --search "error"

## Clean Old Logs

To delete logs older than 30 days:

```bash
python src/main.py --clean 30

📂 Project Structure

```bash
journal-archive-tool/
├── src/                  # Source code
│   ├── main.py           # Entry point of the program
│   ├── collector.py      # Log collection
│   ├── storage.py        # Log storage
│   ├── query.py          # Log querying
│   └── manager.py        # Log management (rotation, deletion, etc.)
│
├── tests/                # Unit and integration tests
│   ├── test_collector.py
│   ├── test_storage.py
│   └── test_query.py
│
├── docs/                 # Project documentation
│   └── README.md         # Main README file
│
├── requirements.txt      # Project dependencies
├── .gitignore            # Files to ignore in Git
└── LICENSE               # License file

🤝 Contributing

Contributions are welcome! Here's how you can contribute:

    Open an issue to discuss what you'd like to add or change.

    Fork the project and clone it to your machine.

    Create a new branch:

git checkout -b my-new-feature

Make your changes and push them:

```bash
git add .
git commit -m "Add a new feature"
git push origin my-new-feature

## Open a pull request to propose your changes.

This project is licensed under the MIT License. See the LICENSE file for details.
