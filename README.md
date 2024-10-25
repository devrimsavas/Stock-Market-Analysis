# Stock Market Analysis Tool

This program provides a comprehensive tool for analyzing stock market data using both classical linear regression and an advanced LSTM (Long Short-Term Memory) machine learning model. It combines data visualization, statistical analysis, and predictive modeling in an interactive GUI.

## Features

### Imported Modules
This program uses various libraries for a robust analysis and user experience:
- **tkinter**: For GUI creation.
- **matplotlib**: For data plotting.
- **pandas**: For data manipulation.
- **sklearn**: For linear regression.
- **yfinance**: For fetching stock data.
- **tensorflow**: For LSTM-based stock price prediction.
- **PIL**: For image manipulation (likely used for displaying company logos).

### Data Collection
- **`fetch_data`**: Fetches historical stock price data for a given ticker symbol over a specified period using Yahoo Finance. If the ticker does not exist or is delisted, an error message is displayed.

### Stock Price Analysis
- **`analyze_data`**: Utilizes simple linear regression to predict the next day’s closing price. It also calculates the R-squared value (which measures model fit) and the F-statistic (to test the model’s overall significance).

### LSTM-Based Stock Price Prediction
- **`train_lstm_model`**: Uses an LSTM neural network model to predict the next day’s closing price. The LSTM model is a type of recurrent neural network (RNN) that is well-suited for time-series data prediction.

### GUI Functions
- **`on_lstm_analyze`, `on_analyze`, and `on_submit`**: Respond to GUI events to fetch data, perform analyses, and display predictions or error messages.
- **`plot_data` and `plot_last_month`**: Display stock price data over the past year and the last month, respectively.
- **`on_treeview_double_click`**: Responds to a double-click event on a list of companies to populate the entry field with the selected company’s name.
- **`plot_placeholder`**: Plots a placeholder image/graph in a specified frame.
- **`show_historical_data`**: Displays a historical view of a stock’s data over the past five years.

### Additional Features
- **`display_logo`**: Likely displays the company’s logo based on its ticker symbol (inferred from usage).
- **`exit_app`**: Closes the application.
- **`save_option`**: Likely saves specific data or options for future reference.

### Initialization
The program loads a CSV file, `companies.csv`, containing company names and their ticker symbols, at startup.

## Usage
- **User Input**: Users can input a company name to fetch and display the company’s stock data, predictions, and other relevant information.
- **Company Selection**: Users can view a list of companies, select one, and obtain detailed information about it.
- **Visualization**: The GUI includes sections to display linear regression and LSTM predictions, recent stock data, company logos, and plots for historical stock prices.

## Summary
This stock market analysis tool allows users to visualize historical stock prices, gain statistical insights through linear regression, and predict future prices using LSTM. Its comprehensive feature set provides a solid foundation for anyone looking to analyze stocks in an interactive, data-driven way.
