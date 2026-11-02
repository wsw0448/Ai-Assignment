# Credit Card Fraud Detection (Ai - Assignment)

## About This Project

This project is about exploring credit card transaction data and looking for patterns that might be related to fraud.

I used Python to examine the dataset and compare fraudulent transactions with normal transactions. I wanted to see how the two groups differ in areas such as transaction distance, purchase price, online orders, and payment methods.

This notebook covers the EDA portion of the project. It does not include building or training a machine learning model.

## Dataset

The dataset used in this project is `card_transdata.csv`.

It contains 999 rows and 8 columns.

| Column | Description |
|---|---|
| `distance_from_home` | Distance between the transaction location and the cardholder's home |
| `distance_from_last_transaction` | Distance from the previous transaction location |
| `ratio_to_median_purchase_price` | Transaction amount compared to the median purchase price |
| `repeat_retailer` | Whether the transaction occurred at a previously used retailer |
| `used_chip` | Whether a chip was used |
| `used_pin_number` | Whether a PIN was used |
| `online_order` | Whether the transaction was made online |
| `fraud` | Whether the transaction was fraudulent (1 = Yes, 0 = No) |

## Tools Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

## AI Assistance

I used ChatGPT (GPT-6) to help with parts of the analysis. I mainly used it to generate Python code, suggest ways to explore the data, and create visualizations.

I also included some of the main prompts I used in the notebook so that the AI assistance throughout the project is documented.

## Reflection

Using AI made the analysis process faster and helped me learn different ways to work with Pandas and visualize data. For example, I could ask ChatGPT to create a box plot comparing fraudulent and normal transactions instead of having to figure out the entire code by myself. It also helped me think of questions to investigate, such as whether fraudulent transactions tend to happen farther from the cardholder's home or whether online orders are more common among fraudulent transactions. This gave me more time to focus on looking at the graphs and understanding what the results showed.

At the same time, I learned that I should not trust everything AI generates. If I use code without understanding what it does, I might get incorrect results and not even realize it. For example, I checked the missing values myself using `df.isnull().sum()` because I wanted to make sure the dataset did not contain missing data that could affect the analysis. I also checked the fraud distribution using `value_counts()` to confirm the percentages. Another thing to be careful about is interpreting correlation. A strong correlation does not necessarily mean that one variable causes fraud. I think AI is a useful tool, but I still need to understand the code and statistics behind the results instead of relying on AI for every decision.

## Conclusion

This project helped me get a better understanding of the credit card transaction dataset and some of the differences between fraudulent and normal transactions.

Through the EDA process, I explored the data, checked its quality, compared transaction characteristics, and looked at relationships between variables. These results provide a starting point for understanding credit card fraud, although they do not prove that any specific transaction is fraudulent.
