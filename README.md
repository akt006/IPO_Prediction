# IPO Precision Using ML

## Project Overview
This project aims to predict the opening price of an Initial Public Offering (IPO) using machine learning techniques. The study was conducted as part of the Bachelor of Technology degree requirements at The LNM Institute of Information Technology, Jaipur, under the guidance of Dr. Ashish Kumar Dwivedi.

## Team Members
- Vipul Khandekar - 20uec147
- Akash Tiwari - 20ucc012
- Ankit Gulia - 20ucc015
- Aadesh Malani - 20ucc001

## Abstract
The project addresses the challenge of accurately predicting the opening price of an IPO to assist retail investors in making informed decisions. Current methods are often unreliable, leading to significant financial losses for investors. By analyzing various factors such as previous financial statements, market penetration, and investment values from institutional buyers, this project aims to develop a predictive model that provides more accurate IPO price predictions.

## Data Collection and Preparation
Data was collected from various financial websites using web scraping techniques. The dataset includes information on 494 companies, covering IPOs from September 2006 to April 2022. Key attributes include:
- NII investment value
- QIB investment value
- Issue size
- Issue price band

To address inflation, the data was adjusted to reflect present value.

## Exploratory Data Analysis
The data was visualized to understand relationships between different variables and the IPO opening price. Below are some key findings:

- **Opening Price Vs Issue Price**
  ![Opening Price Vs Issue Price](openingVSissue.png)

- **Opening Price Vs QIB**
  ![Opening Price Vs QIB](openingVSqib.png)

- **Opening Price Vs HNI**
  ![Opening Price Vs HNI](openingVShni.png)

- **Opening Price Vs RII**
  ![Opening Price Vs RII](openingVSrii.png)

## Algorithms Used
1. **Random Imputation**: Used to handle missing data by replacing missing values with random observations from the feature.
2. **Decision Tree**: A non-parametric supervised learning algorithm used for both classification and regression tasks. It works by recursively splitting the data based on the most informative features.
3. **Random Forest**: An ensemble method that builds multiple decision trees and combines their predictions to improve accuracy and reduce overfitting.

## Results
The proposed model was tested using various algorithms, and the performance was evaluated based on accuracy and prediction reliability.

| Algorithms                        | Accuracy | Accuracy Metric Used |
|-----------------------------------|----------|----------------------|
| Random Forest (n_estimators=100)  | 80.56    | accuracy_score       |
| Random Forest (n_estimators=50)   | 77.37    | accuracy_score       |
| KNN (cross val)                   | 61.63    | cross_val_score      |
| KNN (normalized)                  | 74.03    | accuracy_score       |
| Decision Tree (depth=10)          | 60.07    | accuracy_score       |
| Prediction with Intervals         | 68.45    | r2_score             |
| Gradient Boosting                 | 84.5     | gbr.score            |

- **Accuracy of Models Compared**
  ![Accuracy of Models Compared](Accuracy_of_Models_Compared.png)

## Conclusion
The project successfully developed a machine learning model that predicts IPO opening prices with higher accuracy than traditional methods. This model can help retail investors make better-informed decisions, potentially reducing financial losses.

## Acknowledgments
We extend our special thanks to Dr. Ashish Kumar Dwivedi for his support and guidance throughout the project. We also thank the academic setup for providing this learning opportunity.

## Images of Results
- **Random Forest Analysis**
  ![Random Forest Analysis](randomforest.png)

- **Gradient Boosting Analysis**
  ![Gradient Boosting Analysis](gradientboosting.png)

- **KNN Performance**
  ![KNN Performance](knn.png)


This README file provides an overview of the project, including objectives, methodologies, and key results. For detailed information, please refer to the full project report.
