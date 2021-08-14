# Data Science Primer


* **Machine learning** : is a comprehensive approach to solving problems...

* Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.For true machine learning, the computer must be able to learn patterns that it's not explicitly programmed to identify.

* A task is a specific objective for your algorithms.

* Algorithms can be swapped in and out, as long as you pick the right task.

* In fact, you should always try multiple algorithms because you most likely won't know which one will perform best for your dataset.

* The two most common categories of tasks are :

    * Supervised Learning : includes tasks for "labeled" data (i.e. you have a target variable).
        * In practice, it's often used as an advanced form of predictive modeling.

        * Each observation must be labeled with a "correct answer."

        * Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it).

        * Regression is the task for modeling continuous target variables.

        * Classification is the task for modeling categorical (a.k.a. "class") target variables.

    * Unsupervised Learning : includes tasks for "unlabeled" data (i.e. you do not have a target variable).
        * In practice, it's often used either as a form of automated data analysis or automated signal extraction.

        * Unlabeled data has no predetermined "correct answer."

        * You'll allow the algorithm to directly learn patterns from the data (without "supervision").

        * Clustering is the most common unsupervised learning task, and it's for finding groups within your data.

# Exploratory Analysis

* Proper exploratory analysis is about answering questions. It's about extracting enough insights from your dataset to course correct before you get lost in the weeds.

* The purpose of exploratory analysis is to "get to know" the dataset. Doing so upfront will make the rest of the project much smoother, in 3 main ways:

    * You’ll gain valuable hints for Data Cleaning (which can make or break your models).

    * You’ll think of ideas for Feature Engineering (which can take your models from good to great).

    * You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

* exploratory analysis for machine learning should be quick, efficient, and decisive... not long and drawn out!

* First, you'll want to answer a set of basic questions about the dataset:

    * How many observations do I have?

    * How many features?

    * What are the data types of my features? Are they numeric? Categorical?

    * Do I have a target variable?

* correlations : allow you to look at the relationships between numeric features and other numeric features.Correlation is a value between -1 and 1 that represents how closely two features move in unison. You don't need to remember the math to calculate them