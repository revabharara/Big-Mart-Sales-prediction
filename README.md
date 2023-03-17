# 🎯 Big-Mart-Sales-prediction

The Big Market Sales Prediction project involves analyzing a dataset from Kaggle and developing machine learning models to predict sales in the retail industry. The retail industry is highly competitive, and companies are always looking for ways to increase their revenue and market share. By using machine learning algorithms to predict sales, companies can gain insights into consumer behavior and optimize their business strategies.

# 💡 Need of the model

Predicting future sales accurately can help companies improve their revenue and market share, while also reducing costs associated with inventory management and overstocking. Machine learning models such as the ones used in this project can provide a competitive advantage for companies in the retail industry looking to stay ahead of the competition. 

## 📚 About the Dataset

| Column ID  | Column Name | Data type  | Description |
| ------------- | ------------- |------------- | ------------- |
| 0 | Item_Identifier   | Object | Unique identification for each item |
| 1  | Item_Weight  | Float64 | weight of the item  |
| 2  | Item_Fat_Content  | Object | amount of fat in the item  |
| 3  | Item_Visibility  | Float64 | Visibility of the item as comapared to others  |
| 4  | Item_Type  | Object | The category that an item falls under  |
| 5  | Item_MRP  | Float64 | retail price of the item  |
| 6  | Outlet_Identifier   | Object | Unique outlet identification for each outlet  |
| 7  | Outlet_Establishment_Year  | int64 | year the outlet was established in  |
| 8  | Outlet_Size  | Object | size of the outlet  |
| 9  | Outlet_Location_Type  | Object | category of location that the outlet falls under  |
| 10  | Outlet_Type  | Object | type of outlet  |
| 11  | Item_Outlet_Sales  | Object | average sales of item in outlet  |

We also have a testing dataset that had similar columns but the target i.e. Item_Outlet_Sales is missing.

# 🛣️ Roadmap for the project

## 🔭 Data exploration
In this section we will explore the datasets and figure out its features and characteristics.

We can gather the following insights after exploration:
1. there are null values in both te testing and training datasets.
2. there are several categorical values that we will need to encode for prediction and model fitting.

## ⚙️ Data Preprocessing:
In this section we will:
1. *Clean the data*
    * We will be replacing the missing numerical values with the mean of the column.
    * We will be replacing the categorical missing data with the mode of that particular category.
  
2. *Extract the features*
    Here we will be encoding the features using label encoding so that the data is easier to process and use. We use the LabelEncoder from sklearn that assigns a unique number to each unique value in the column.
    
3. *Standardize and Normalize the data if needed*
    In this step we will be standardising tyhe data so that there are no redunadant as well as values that mean the same thing but under different names (e.g. 'lf', 'low fat', 'Low Fat' all mean the same thing.)

## 	📊 Data analysis
In this section I will:

1. Finding correlations between different variables

<img width="480" alt="image" src="https://user-images.githubusercontent.com/89579327/225888942-58299450-0326-486d-9be9-6ddc85045665.png">

2. See the distribution of items in various categories based on the respective columns

<img width="735" alt="image" src="https://user-images.githubusercontent.com/89579327/225889254-7f70980c-76e1-4101-a9af-f655a44e6296.png">

<img width="327" alt="image" src="https://user-images.githubusercontent.com/89579327/225889306-40ae3ee3-58fa-46c8-99d7-b2f32681542f.png">


3. plotting some regression correlations.

<img width="379" alt="image" src="https://user-images.githubusercontent.com/89579327/225889060-15771a3a-a6ea-4c7c-9146-a9595671a4b7.png">

<img width="393" alt="image" src="https://user-images.githubusercontent.com/89579327/225889170-cbe36805-f5eb-4aee-9757-363ff508958a.png">

## ⛳ Model Selection and Prediction

In this section we will be trying different regression models and see which one gives us the best results in terms of minimizing the error in its prediction.

### The models we will use are:

1. Simple Linear Regression
2. Multiple Linear Regression
3. Polynomial regression
4. Random Forest Regression
5. XGBoost regression

### 🏆Model Comparison
In this section we will be comparing the differnt models implemented in the previous sections to find what works best. This involves:

1. comparing based on errors and accuarcy scores

<img width="554" alt="image" src="https://user-images.githubusercontent.com/89579327/225890116-2b919cb8-e888-435a-b2f2-20788acb7fcd.png">

2. plotting them to find the best model

![image](https://user-images.githubusercontent.com/89579327/225890145-37d69745-73cf-45a0-9523-9bff4b2259b4.png)

### 🎍Conclusion:
In conclusion, the Big Market Sales Prediction project involved analyzing a dataset from Kaggle and developing machine learning models to predict sales in the retail industry. Five different models were tested, including linear regression, multiple regression, polynomial regression, random forest regressor, XGBoost regressor. The evaluation of the models was based on the R2 score, Mean Absolute Error (MAE), and Mean Squared Error (MSE).

After testing the models, it was found that the polynomial regressor with degree 3 performed the best in predicting sales. This model had the highest R2 score and the lowest MAE and MSE. It can be concluded that this model is the most accurate in predicting future sales in the retail industry.

### 🗻Applications:
The findings of this project can be valuable for companies in the retail industry looking to forecast sales and optimize their business strategies. By utilizing machine learning models such as the polynomial regressor with degree 3, companies can gain insights into consumer behavior and make informed decisions to improve their bottom line. Overall, this project demonstrates the potential of machine learning in predicting sales and its impact on the retail industry.

### 🧮 Limitations:
1. Dataset limitations: The project relied on a specific dataset from Kaggle, which may not be representative of all retail industries. Differences in products, consumer behavior, and regional factors may affect the accuracy of the predictions.

2. External factors: Predicting sales accurately may be affected by external factors such as economic trends, competitor activities, and changes in consumer behavior, which may not be captured by the models.

3. Model performance: While the polynomial regressor with degree 3 was found to be the most accurate model for predicting sales, it may not perform as well on different datasets or in different time periods.

### 🔮 Future Prospects:

1. Incorporation of external factors: Future iterations of the project could include additional features that capture external factors such as competitor activities or economic trends to improve the accuracy of the predictions.
2. Application to different industries: While the project focused on the retail industry, the same methodology could be applied to other industries where sales forecasting is important, such as healthcare or finance.
3. Deployment as a web application: The models could be deployed as a web application, allowing businesses to input their own data and obtain sales predictions in real-time without requiring extensive knowledge of machine learning techniques.

### 👩‍🦱 Credits:
Reva Bharara

Email : revabharara@gmail.com, bhararareva@gmail.com

Linkedin : https://www.linkedin.com/in/reva-bharara-a83a78241/
