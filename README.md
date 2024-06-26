![Contributors][contributors-shield]
![Forks][forks-shield]
![Stargazers][stars-shield]
![Issues][issues-shield]
![flask-url][flask-badge]
![python-url][python-badge]
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/98084a8c9b46418b82f3dc3cc80bcd26)](https://app.codacy.com/gh/SinghAstra/Stock-API/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)

# Stock API

<p>This API allows to fetch stock price and related information for a given stock ticker and exchange..</p>

<div align="center">
  <a href="https://stock-api-gbbj.onrender.com"><img src="https://github.com/SinghAstra/Stock-API/blob/main/images/trading.png"/></a>
</div>

# Technologies

- Flask
- Python

### Installation

1. Clone the repository:
   ```console
       git clone https://github.com/SinghAstra/Stock-API.git
   ```
2. Install dependencies:
   ```console
       pip install -r requirements.txt
   ```

### Usage

1. Run the flask server:
   ```console
   python app.py
   ```
2. Access the API at http://localhost:5000/

### EndPoints

- **GET /stock_price** : Fetches stock price and related information for a given stock ticker and exchange.
  - **Query Parameters**:
    - ticker: The stock ticker symbol (required)
    - exchange: The stock exchange (required)
    - Example Request :
      ```console
      https://stock-api-gbbj.onrender.com/stock_price?ticker=GOOG&exchange=NASDAQ
      ```
      - Example Response :
      ```console
      {
      "Avg Volume": "20.96M",
      "Day range": "$151.08 - $154.84",
      "Dividend yield": "-",
      "Market cap": "1.90T USD",
      "P/E ratio": "28.37",
      "Previous close": "$151.94",
      "Primary exchange": "NASDAQ",
      "Stock Price": "$153.94",
      "Year range": "$103.27 - $157.00"
      }
      ```
- **GET /** - Welcome message.

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/SinghAstra/Stock-API.svg?style=for-the-badge
[contributors-url]: https://github.com/SinghAstra/Stock-API/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/SinghAstra/Stock-API.svg?style=for-the-badge
[forks-url]: https://github.com/SinghAstra/Stock-API/network/members
[stars-shield]: https://img.shields.io/github/stars/SinghAstra/Stock-API.svg?style=for-the-badge
[stars-url]: https://github.com/SinghAstra/Stock-API/stargazers
[issues-shield]: https://img.shields.io/github/issues/SinghAstra/Stock-API.svg?style=for-the-badge
[issues-url]: https://github.com/SinghAstra/Stock-API/issues
[flask-url]: https://flask.palletsprojects.com/en/3.0.x/
[python-url]: https://www.python.org/
[flask-badge]: https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white
[python-badge]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
