Aim :
Perform data preprocessing tasks and Demonstrate performing association rule mining on data sets
Data Preprocessing in Weka
•	Applying Discretization Filter
•	Discretization converts numeric attributes into nominal ranges.

•	This helps algorithms like Apriori which require categorical inputs



•	Weka provides supervised and unsupervised discretization filters.
 
 

•	The filter can be applied from the Preprocess panel.

•	Discretization improves interpretability in association rules.

•	Applying Resample Filter
•	Resample filter is used for random sampling of instances.
 
 
•	It can be applied with or without replacement.

•	It helps in balancing datasets with class imbalance.

•	Users can specify the percentage of data to retain.
•	Resampling improves fairness in classification and rule mining.
 
 
•	Other Filters in Weka
•	Weka provides Normalize and Standardize filters for scaling data.

•	Attribute removal filter allows removing unwanted fields.
•	Replace missing values filter is used for data cleaning



•	Nominal to Binary filter converts nominal attributes into binary form.
 
 
•	These filters enhance the quality and usability of data.

Association Rule Mining in Weka
•	Running Apriori on Weather Dataset
•	Open weather.nominal dataset in Weka.

•	Select Associate → Apriori algorithm.
 
 
•	Run with default support (0.1) and confidence (0.9).

•	Apriori generates rules like “If Outlook=Sunny then Play=No.”
•	Rules represent hidden relationships among attributes.



•	Running Apriori on Iris Dataset
 
•	Open iris.arff dataset in Preprocess panel.

•	Apply discretization filter to convert numeric attributes.

•	Run Apriori algorithm with minimum support 0.2 and confidence 0.8.

•	Generated rules include attribute-value relations for flower types.
 
 
•	Discretization helps Apriori produce meaningful categorical rules
2.	Running Apriori on Glass Dataset
•	Load glass.arff dataset into Weka.

•	Since Glass has many numeric attributes, apply discretization.

•	Run Apriori with lower support (0.05) due to large attribute set.
 
 
•	Generated rules may highlight chemical compositions linked to glass type.

•	Insights help identify key features that differentiate glass categories.

Effect of Discretization in Rule Generation
•	Without Discretization
 
•	Numeric attributes make rule generation difficult.


•	Apriori may fail to produce useful rules.
•	Continuous values reduce chances of frequent patterns.

•	Rules may be very specific with little generalization.
•	Insights are limited and harder to interpret.
 
 
•	With Discretization
•	Numeric attributes are converted into ranges (bins).

•	Frequent patterns become easier to detect.

•	Rules become simpler and more interpretable.
•	Support and confidence of rules improve.
 
 
•	Discretization clearly enhances Apriori performance.
Insights and Observations
•	Preprocessing improves the quality of data for mining tasks.

•	Discretization significantly helps in Apriori rule generation.

•	Weather dataset gives simple and interpretable rules.
 
 
•	Iris and Glass datasets generate complex rules after discretization.

•	Overall, Apriori with discretized attributes produces more meaningful insights.
Before Decritization:

After Decritization:
 
 

