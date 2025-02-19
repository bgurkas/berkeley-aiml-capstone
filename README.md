### Enhanced Media Recommendation

**Author: Beril Gurkas**

#### Executive summary: A media recommendation system that incorporates multiple factors such as genre, mood tags, and prior ratings

#### Rationale
As a user of media streaming platforms that incorporate recommender systems, some of their recommendations based on genre are pretty accurate. However, I would like to have the power to ask the media streaming platform about media that I feel like watching at that moment (it might be different from what I have been watching before/recently) without having to ask a search engine, since the media streaming platform would know my taste in media better than the search engine.

#### Research Question
Can we build a media recommendation system that incorporates multiple factors such as genre, mood tags, and prior ratings to provide better recommendations to media service users and improve user retention?

#### Data Sources
The MovieLens 100K dataset found [here](https://grouplens.org/datasets/movielens/). 

#### Methodology
- Dimensionality reduction
- Clustering to build user profiles
- SURPRISE Library for recommender systems

#### Results
- Ratings for the Movie IDs associated with each movie were found to be sparse. Not every Movie ID had been rated, and ratings seem centered around Movie IDs 0-12500.
- Genre data seems to be heavily imbalanced in favor of more Drama and Comedy movies compared to other genres. This will introduce a bias if the model produced with this dataset were to be applied to a more balanced dataset.
- The ratings don't seem to be correlated too heavily with any of the genres.

#### Next steps
Include the user-defined tags in the predictions.

Incorporate a bigger dataset, like the MovieLens 1M dataset, which also includes information about how strongly the user-defined tags relate to the movies they rated.

#### Outline of project

- [Initial Exploration](eda.ipynb)


##### Contact and Further Information
- bgurkas@uci.edu