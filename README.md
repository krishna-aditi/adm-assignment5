### Retail Revenue Generated by Customers

- The Streamlit app directly interacts with the data stored on Snowflake. The predicted revenue is also stored in the database. Every time the user adds a new data point using the sliders on the app, a look up is performed to retrieve the average revenue that was predicted to be fetched from the data stored in the database based on the input conditions.
- A Plotly plot is also generated using K-Means algorithm which breaks down the data into 3 clusters - high revenue, medium revenue, low revenue customers.
- Based on the synthetically generated user, five similar customers from the static dataset are retrieved as a dataframe, based on a user defined function (UDF). We also made use of libraries like AgGrid, and Plotly to beautify the Streamlit interface.
- The similar customers are estimated using Euclidean Distance and K-Nearest Neighbors.

#### Running the App
```
streamlit run streamlitapp.py
```
#### Preview
![Streamlit - Page 1](https://github.com/krishna-aditi/adm-assignment5/blob/main/report/screenshot_2.PNG)
![Streamlit - Page 2](https://github.com/krishna-aditi/adm-assignment5/blob/main/report/screenshot_1.PNG)





