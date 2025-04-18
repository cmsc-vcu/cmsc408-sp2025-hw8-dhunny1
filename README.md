# cmsc408-sp2025-hw8: World Bank Indicator Analysis

**Author:** Hunny Biguvu
**Published:** April 18, 2025
**GitHub Repository:** [https://github.com/cmsc-vcu/cmsc408-sp2025-hw8-dhunny1]

## Overview

This repository contains the files and analysis conducted for Homework 8 of the CMSC 408 (Database Systems) course at VCU, Spring 2025. The primary objective of this assignment is to utilize SQL for the exploration and analysis of a World Bank indicators dataset, specifically the `world_bank_data` database. Through a series of analytical questions and data transformations, this project aims to derive meaningful insights from the provided information.

## Project Structure

The repository is organized with the following files:

* `README.md`: This file, serving as the entry point and providing a comprehensive overview of the project.
* `homework8.qmd`: The Quarto document that encompasses the Python code and the SQL queries executed for the data analysis.
* `helpers.py`: A Python script containing utility functions designed to facilitate database connectivity and SQL query execution, as referenced in the problem background.
* `.env`: A configuration file (intentionally excluded from version control) that securely stores the necessary database connection credentials.

## Setup and Execution

To replicate and execute this analysis, the following prerequisites must be met:

1.  **Python 3.x:** Ensure that Python version 3 or higher is installed on your local machine.
2.  **Quarto CLI:** Install the Quarto command-line interface, which is required to render the `homework8.qmd` document. Instructions for installation can be found on the [Quarto website](https://quarto.org/docs/install/).
3.  **Python Libraries:** Install the necessary Python packages, including `pymysql` for MySQL database interaction and potentially other libraries utilized by the `helpers.py` script. These can be installed using pip:

    ```bash
    pip install pymysql cryptography poetry
    ```
4.  **Poetry Environment:** Initialize and enter the Poetry shell to manage project dependencies:

    ```bash
    poetry shell
    ```
5.  **Repository Files:** Clone the necessary files from the GitHub repository to your local environment:

    ```bash
    git clone [https://github.com/cmsc-vcu/cmsc408-sp2025-hw8-dhunny1](https://github.com/cmsc-vcu/cmsc408-sp2025-hw8-dhunny1)
    ```
6.  **`.env` Configuration:** Create a `.env` file in the root directory of the project and populate it with your specific database connection details, adhering to the following structure:

    ```
    CMSC408_HW8_USER="your_db_username"
    CMSC408_HW8_PASSWORD="your_db_password"
    CMSC408_HW8_HOST="your_db_host"
    CMSC408_HW8_DB_NAME="your_db_name"
    ```

    **Important:** For security reasons, ensure that the `.env` file is not committed to any public version control system.
7.  **Database Access:** Verify that you have the necessary access to the `world_bank_data` database as specified in the `.env` file.

Once the setup is complete, the analysis and report generation can be performed by rendering the Quarto document (`homework8.qmd`) using the Quarto CLI:

```bash
quarto render homework8.qmd
```