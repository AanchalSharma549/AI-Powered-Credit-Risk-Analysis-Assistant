# AI-Powered Credit Risk Analysis Assistant

## Project Overview

This project is an AI-powered Credit Risk Analysis Assistant built using **SQL, Python, MySQL, Pandas and Google's Gemini API**.

The assistant analyses loan portfolio data and allows users to ask credit risk-related questions in natural language. Gemini identifies the appropriate analytical tool, Python executes the corresponding SQL query on the MySQL database, and the results are presented in an easy-to-understand format.

## Key Features

The project includes 11 credit risk analysis tools:

1. Customer Exposure Analysis
2. Delinquency and Payment Health Analysis
3. High-Risk Customer Identification
4. Sector Concentration Analysis
5. Geographic Risk Distribution
6. Loan-to-Value (LTV) Risk Analysis
7. Payment Trend Analysis
8. Vintage Analysis
9. Customer Risk Scoring
10. Key Risk Indicators (KRI) Dashboard
11. Defaulted Loan Identification

## Technologies Used

- **SQL (MySQL):** Data retrieval, joins, aggregations and credit risk analysis.
- **Python:** Database connectivity and application logic.
- **Pandas:** Data handling and analysis.
- **Google Gemini API:** Natural language understanding and function calling.
- **Jupyter Notebook:** Development and testing.

## How It Works

1. The user asks a credit risk-related question in natural language.
2. Gemini identifies the relevant analytical function.
3. Python executes the corresponding SQL query.
4. MySQL retrieves the required loan portfolio information.
5. Gemini interprets the returned results and generates a simple response.

## Credit Risk Metrics

The project analyses several important credit risk indicators, including:

- Loan Exposure
- Days Past Due (DPD)
- Loan-to-Value (LTV)
- Credit Scores
- Default Rates
- Payment Behaviour
- Portfolio Concentration
- Customer Risk Scores

The customer risk scoring tool uses a weighted analytical formula based on credit score, average LTV, average DPD and default history.

## Project Structure

```text
AI-Credit-Risk-Assistant/
│
├── connector.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Setup and Requirements

### Prerequisites

- Python
- MySQL Server
- A MySQL database named `credit_risk_db`
- The required database tables and loan portfolio data
- A Google Gemini API key

### Installation

Install the required Python libraries:

```bash
pip install pandas mysql-connector-python python-dotenv google-genai requests
```

### Environment Variables

Create a `.env` file in the project directory:

```text
DB_USER=your_mysql_username
DB_PASSWORD=your_mysql_password
GEMINI_API_KEY=your_gemini_api_key
```

The notebook expects the MySQL database to be available locally and uses the database name `credit_risk_db`.

### Running the Project

1. Set up the MySQL database and required tables.
2. Add your database credentials and Gemini API key to `.env`.
3. Install the required libraries.
4. Open `connector.ipynb` in Jupyter Notebook.
5. Run the notebook cells in order.
6. Ask credit risk-related questions using the assistant.

## Important Note

This project is an educational portfolio project demonstrating SQL-based credit risk analysis and AI integration. The customer risk scoring formula is an illustrative analytical scoring approach and is not a statistically validated Probability of Default model.

The database schema and sample data must be configured separately before running the notebook.
