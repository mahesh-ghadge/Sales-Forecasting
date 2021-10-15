# Sales-Forecasting
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/heading.PNG)
## Description
A multinational retail corporation operates the chain of hypermarkets, discount department stores and grocery stores all around the world.  Presently the company has to rely on outdated manual sales forecasting techniques to predict the weekly sales of stores.  So they want to automate this task to predict weekly sales of their stores.

We have provided historical data for stores located in different regions. Each store contains a number of departments and the goal was to predict the sales department wise.

### Steps followed on given dataset

- We studied **in-depth** about the various **features** in the data, their **characteristics** and their **distributions**.

- We went through an **extensive** and **thorough** data analysis process, exploring various **questions** regarding the **relation** between the **weekly sales** of the stores and their different **features**.
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/Distribution%20of%20Type.png)
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/Relationship%20Between%20the%20Size%20and%20Type%20of%20the%20Store.png)
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/Relationship%20Between%20the%20Weekly%20Sales%20and%20Type%20of%20the%20Store.png)
- We **encoded** the *categorical data* and **removed** any *redundant columns* to make our dataset fit for training.

- We created some **baseline models** and fitted them with the **entire dataset** and compared their performace.

- The **Baseline Random Forest** model was the **best** baseline model with **least RMSE** value.

- Then with the help of Random Forest we **compared** the **importance** of each feature in the dataset, and selected the **top 6** *most important features*.
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/Feature%20Importance%20of%20each%20Feature.png)
- In this way,  the Random Forest model helped us in **Feature Selection** for our Essential Feature Models.

- We then created the **Essential Feature Models** and fitted them using only the **top 6 most important features**.
  
- The models performed much **better** after **removing** the *non-essential features*, and the **Essential Feature Random Forest** model was the **best model** overall with the **least RMSE** score of all models.
![enter image description here](https://raw.githubusercontent.com/mahesh-ghadge/Sales-Forecasting/main/images/Model_comparision.PNG)
- We **tuned** the **hyperparameters** for our Random Forest model using **Grid Search** and further improved it's performance.

- We selected the **best hyperparameter combination** model found using Grid Search as our **final model**, and made **predictions** on the test set using it.

- Our final model gave a **R-Squared** value of **0.98** on the *test set*, implying that it is indeed a **very good model**, and is generalizing well on unseen data.
