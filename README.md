# Problem
There is a list of companies of both Venture Capital and Non Venture capital. Now, need to build a model based on a list so that to  predict if the company is a venture capital firm or not

# Data Exploration
I have combined the data in a single sheet then shuffle the data 
For this prjoect we have only three columns ie company_name,url,category

Target is "category"

![Capture.PNG](https://github.com/Saithretha/Venture_Capital/blob/master/resource/Capture.PNG)

# Text Representation
The classifiers and learning algorithms can not directly process the text documents in their original form, as most of them expect numerical feature vectors with a fixed size rather than the raw text documents with variable length. Therefore, during the preprocessing step, the texts are converted to a more manageable representation.

Specifically, for each term in our dataset, we will calculate a measure called Term Frequency, Inverse Document Frequency, abbreviated to tf-idf. We will use sklearn.feature_extraction.text.TfidfVectorizer to calculate a tf-idf vector for company name

![Capture.PNG](https://github.com/Saithretha/Venture_Capital/blob/master/resource/Capture1.PNG)

# Model Building
MultinomialNB is giving good results when compared to other models

![Capture.PNG](https://github.com/Saithretha/Venture_Capital/blob/master/resource/Capture3.PNG)

![Capture.PNG](https://github.com/Saithretha/Venture_Capital/blob/master/resource/Capture4.PNG)
