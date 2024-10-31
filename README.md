E-commerce Platform Price Optimization

**Introduction**  
Price optimization is a fundamental aspect of e-commerce, leveraging historical sales data to identify trends and anomalies in product transactions. The objective is to predict an ideal price point that balances customer purchase likelihood with company profit margins. This project applies various machine learning algorithms to historical data to generate a demand curve, identifying a price that maximizes sales volume and profitability for a given product.

**Dataset**  
The project utilizes the publicly available Brazilian e-commerce dataset, which consists of transaction records from the Olist store in Brazil. Spanning from 2016 to 2018, the dataset includes over 100,000 entries and around 40 features. Only records with a "delivered" order status are considered to ensure data relevancy for the analysis.

**Methodology**  
This project follows a five-step process:

1. **Data Cleaning and Preprocessing**  
   The dataset is cleaned to remove irrelevant and duplicate entries, and features like year, month, and year-month are extracted from timestamps. Filtering is done to retain only "delivered" orders, and an "order_count" column is added to measure sales volume.

2. **Dimensionality Reduction**  
   Principal Component Analysis (PCA) is employed to reduce the data's dimensionality, transforming it from a high-dimensional to a more manageable space while retaining significant features. PCA is applied to 24 features, reducing them to 17 components after categorical features are encoded with Label Encoding.

3. **Exploratory Data Analysis**  
   Analysis is conducted to uncover insights on aspects like product categories, sales trends, and revenue generation. Key findings include temporal patterns in order counts, top revenue-generating categories, and sales peaks during events like Black Friday.

4. **Modeling**  
   Models are trained using Linear Regression, Ridge, and Lasso regression algorithms to estimate price. Evaluation metrics include Mean Squared Error (MSE), with the project also incorporating a profit function and generating a demand curve to estimate optimal prices for specific products.

5. **Results and Discussion**  
   The analysis suggests that adjusting the price of a particular product (ID: 437c05a395e9e47f9762e677a7068ce7) from $50.03 to $39.59 may boost sales volume by 45%, potentially increasing revenue by 78%. The project suggests further enhancements through advanced techniques, such as neural networks or hybrid models.

**Conclusion**  
While linear regression shows potential in optimizing pricing, more complex techniques like neural networks may yield further improvements. This project underscores the importance of price optimization in driving e-commerce sales and profitability.
