# Bitcoin Trader Sentiment Analysis

This project analyzes how trader performance changes with Bitcoin market sentiment.

The main idea is to compare trading results during different market moods like:

- Extreme Fear
- Fear
- Neutral
- Greed
- Extreme Greed

## Files

- `trader_sentiment_analysis.ipynb` - Main Jupyter Notebook with code, charts, and insights.
- `bitcoin_trader_report.html` - HTML version of the final report.
- `DataSet/fear_greed_index.csv` - Bitcoin Fear and Greed sentiment data.
- `DataSet/historical_data.csv` - Trader historical trading data.

## What I Did

- Loaded and cleaned both datasets.
- Converted timestamps into proper dates.
- Merged trader data with sentiment data using date.
- Calculated PnL, win rate, trade count, and trade size by sentiment.
- Found top and bottom traders.
- Compared performance during Fear and Greed markets.
- Checked Extreme Fear vs Extreme Greed performance.
- Created charts using matplotlib and seaborn.

## Main Findings

- Trader performance changes across different sentiment conditions.
- Extreme Greed had strong average and realized PnL.
- Extreme Fear showed higher downside risk.
- Many trades had zero closed PnL, so realized PnL rows were checked separately.
- The dataset did not contain a direct leverage column, so trade size and starting position were used as risk indicators.

## How to Run

1. Open `trader_sentiment_analysis.ipynb` in Jupyter Notebook.
2. Run the cells from top to bottom.
3. Make sure the `DataSet` folder is in the same project directory.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn

## Conclusion

This analysis shows that Bitcoin market sentiment can help explain trader behavior and performance. It also shows that risk and consistency are important, not just total profit.
