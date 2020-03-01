# Problem Formulation
The list consist of data of companies of venture capital and non venture capital. Now, need to build a model that, based on a company website, can predict if the company is a venture capital firm or not

# Data Exploration
For this prjoect we have only three columns ie company_name,url,category
Target is "category"

![Capture.PNG](https://raw.github.com/Saithretha/Venture_Capital/resources/Capture.PNG)

# Text Representation
The classifiers and learning algorithms can not directly process the text documents in their original form, as most of them expect numerical feature vectors with a fixed size rather than the raw text documents with variable length. Therefore, during the preprocessing step, the texts are converted to a more manageable representation.

Specifically, for each term in our dataset, we will calculate a measure called Term Frequency, Inverse Document Frequency, abbreviated to tf-idf. We will use sklearn.feature_extraction.text.TfidfVectorizer to calculate a tf-idf vector for each of consumer complaint narratives:

# Model Building
MultinomialNB is giving good results
