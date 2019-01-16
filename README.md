# Music Artist Recommender System

Built a personalized music artist recommendation system with Yahoo! music community ratings.

### Data

### Steps
First I Performed online analytical processing (OLAP) based on Spark Dataframe and Spark SQL.

Then Trained ALS model based on Collaborative Filtering in PySpark MLlib and tuned hyperparameters with cross-validation toolbox.
The Spark API provides the implementation of the ALS algorithm, which is used to learn these latent factors based on the following six parameters:
- ```numBlocks```: The number of blocks used to parallelise computation (set to -1 to auto-configure).
- ```rank```: The number of latent factors in the model.
- ```iterations```: The number of iterations of ALS to run. ALS typically converges to a reasonable solution in 20 iterations or less.
- lambda: The regularisation parameter.
- implicitPrefs: Whether to use the explicit feedback from the ALS variant for implicit feedback data.
- alpha: A parameter applicable to the implicit feedback variant of ALS that governs the baseline confidence in preference observations.
