# Assignment 1: Log and Reflection

## 1. Checking AI Suggestions
I evaluated the alternative questions proposed by the AI coach against the variables available in the data dictionary (`item`, `price`, `city`, `date`). 

* **Accepted Alternative 2:** Checking if a specific item became cheaper over time. (Supported by tracking `price`, `item`, and `date`).
* **Accepted Alternative 3:** Checking if the two cities trade places regarding which is more expensive over time. (Supported by tracking `price`, `city`, and `date`).

### Rejected Alternatives
* **Rejected Alternative 1 (Volatility):** Rejected because tracking week-over-week volatility requires complex statistical variance modeling that goes beyond the basic descriptive nature of this pricing dataset.
* **Rejected Alternative 4 (Luxury Item Skew):** Rejected because the dataset contains basic commodity staples, not high-end luxury goods, so checking for a luxury-driven skew is irrelevant to this data dictionary.
* **Rejected Alternative 5 (Percentage Growth Rates):** Rejected because the data logs raw nominal prices rather than indexed rates, making flat price tracking a cleaner approach for answering the core claims.
## 2. Reflection on Data Capabilities
This dataset is fully capable of showing direct price trajectories, cross-city price disparities, and temporal commodity trends over a fixed six-month window. By sorting and filtering the nominal prices across the discrete city and item columns, I can definitively answer whether one city remains systematically more expensive or if specific items experience seasonal declines. 
However, this data cannot explain the underlying economic factors, inflation root causes, or supply chain disruptions causing these fluctuations. It tracks what the prices are, but it lacks the contextual variables required to declare why they are changing.
## 3. The Unsupported Temptation Trap
The most tempting suggestion was Alternative 5, which proposed analyzing the percentage growth rates of price changes across both cities. This suggestion is completely unsupported because our data dictionary only provides flat, raw nominal prices without any pre-calculated indices or volume weights. Trying to extrapolate broader relative inflation speeds from a small, isolated list of four basic items would create misleading macroeconomic conclusions not supported by this dataset.