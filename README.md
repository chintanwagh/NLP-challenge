# NLP-Brand Name Extraction from Product List using Naive Bayes Classifier

-You’ve been given a product list of ~16,000 carbonated soft drinks (see carbonated_soft_drinks.csv) and you’re asked to build a model that can extract the product’s brand (e.g., Coke, Pepsi Sunkist), when available. 
### Product List Brand Classifier
This is a Python script that uses supervised machine learning to classify soft drinks in a product list dataset based on their brand names.

### Prerequisites
Python 3.6 or higher
pandas library
scikit-learn library
### How it works
The script performs the following steps:

Load the product list data from a CSV file using pandas.
Define a list of known brand names.
Define a function that extracts the brand name from the item name using regular expressions.
Add a new column to the DataFrame to store the extracted brand names.
Remove rows with missing brand names.
Split the data into training and testing sets.
Vectorize the training and testing data using the CountVectorizer class from scikit-learn.
Train a Naive Bayes classifier on the training data using the MultinomialNB class from scikit-learn.
Evaluate the accuracy of the classifier on the testing data.
extract the new file to csv which includes brand names

### How to use

Install the required libraries using pip:
pip install pandas scikit-learn
Place your product list CSV file in the same directory as the script.
Edit the script to use the correct file name:

df = pd.read_csv("carbonated_soft_drinks.csv")

### Run the script:

NLP_Challenge_part2.ipynb

### Results
carbonated_soft_drinks_with_brands.csv

The script will output the accuracy of the classifier.
