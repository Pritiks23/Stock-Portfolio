
The **Top 12 Crypto Portfolio Tracker** is a web application that allows users to monitor the top 12 cryptocurrencies by market capitalization. Users can input the amount of each cryptocurrency they own and calculate the total value of their portfolio in USD. Prices are fetched in real-time from the CoinGecko API.

<img width="952" height="756" alt="Screen Shot 2025-09-01 at 11 13 42 AM" src="https://github.com/user-attachments/assets/0fdb2afa-0c8f-43d3-8b6c-8ae8c183d378" />


Try me here: https://pritiks23.github.io/Stock-Portfolio/

## Features
- Dynamic retrieval of top 12 cryptocurrencies sorted by market cap.
- Real-time USD price updates via CoinGecko API endpoints.
- User input for holdings with automatic calculation of portfolio value.
- Responsive design with a semi-transparent overlay for optimal readability on background imagery.
- Minimal dependencies for ease of deployment.

## Architecture & Implementation
- **Frontend:** Built entirely with vanilla HTML, CSS, and JavaScript.
- **Data Fetching:** Utilizes `fetch()` API to interact with CoinGecko endpoints:
  - `GET /coins/markets` for retrieving market data (name, symbol, price, market cap)
  - `GET /simple/price` for updating individual coin prices
- **Data Binding:** DOM manipulation with `document.createElement()` and `innerHTML` for dynamic table generation.
- **Event Handling:** Real-time updates via `input` events on amount fields, recalculating portfolio value without page reload.
- **Styling:** CSS overlays (`rgba`) ensure visibility of text over background images while maintaining modern UI aesthetics.

## Technologies Used
- HTML, CSS, and JavaScript
- CoinGecko API for cryptocurrency prices
- Google Fonts (Roboto) for typography

