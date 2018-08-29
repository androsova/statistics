## Movie score prediction

### Linear regression approach (https://htmlpreview.github.io/?https://github.com/androsova/movie_score_prediction/blob/master/reg_model_project.html)

#### Instructions

Your boss has just acquired data about how much audiences and critics like movies as well as numerous other variables about the movies. This dataset is provided below, and it includes information from Rotten Tomatoes and IMDB for a random sample of movies.

She is interested in learning what attributes make a movie popular. She is also interested in learning something new about movies. She wants you team to figure it all out.

As part of this project you will complete exploratory data analysis (EDA), modeling, and prediction.

All analysis must be completed using the R programming language via RStudio, and your write up must be an R Markdown document. 

#### Information on the data

The data set is comprised of 651 randomly sampled movies produced and released before 2016.

Some of these variables are only there for informational purposes and do not make any sense to include in a statistical analysis. It is up to you to decide which variables are meaningful and which should be omitted. For example information in the the `actor1` through `actor5` variables was used to determine whether the movie casts an actor or actress who won a best actor or actress Oscar.

You might also choose to omit certain observations or restructure some of the variables to make them suitable for answering your research questions.

When you are fitting a model you should also be careful about collinearity, as some of these variables may be dependent on each other.

Source of information: Rotten Tomatoes (https://www.rottentomatoes.com) and IMDB (http://www.imdb.com) APIs.

#### Information on model selection

You may choose to use any of the model selection techniques presented in this course, however you should justify your choice. Note that there are many other model selection techniques that are beyond the scope of this course, and those should not be used in this project.

Regardless of whether you are doing forward selection or backward elimination, you should decide on a set of variables that will be considered for the model. These do not have to include all of the variables in the dataset. In fact, some variables might be completely inappropriate to consider (such as URL of the movie) or clearly not informative (such as the actor variables with so many levels). You should first go through the dataset and identify the variable you want to consider, and provide a justification for including those (or excluding the others).


### Bayesian statistics approach (https://htmlpreview.github.io/?https://github.com/androsova/movie_score_prediction/blob/master/bayesian_project.html)

#### Instructions

Your boss has just acquired data about how much audiences and critics like movies as well as numerous other variables about the movies. This dataset is provided below, and it includes information from Rotten Tomatoes and IMDB for a random sample of movies.

Your boss is interested in learning what attributes make a movie popular. She is also interested in learning something new about movies. She wants your team to figure it all out.

As part of this project you will complete exploratory data analysis (EDA), modeling, and prediction.

The specific modeling task you need to complete is as follows: Develop a Bayesian regression model to predict audience_score from the following explanatory variables. Note that some of these variables are in the original dataset provided, and others are new variables you will need to construct in the data manipulation section using the mutate function in dplyr:

- feature_film: "yes" if title_type is Feature Film, "no" otherwise
- drama: "yes" if genre is Drama, "no" otherwise
- runtime
- mpaa_rating_R: "yes" if mpaa_rating is R, "no" otherwise
- thtr_rel_year
- oscar_season: "yes" if movie is released in November, October, or December (based on thtr_rel_month), "no" otherwise
- summer_season: "yes" if movie is released in May, June, July, or August (based on thtr_rel_month), "no" otherwise
- imdb_rating
- imdb_num_votes
- critics_score
- best_pic_nom
- best_pic_win
- best_actor_win
- best_actress_win
- best_dir_win
- top200_box

All analysis must be completed using the R programming language via RStudio, and your write-up must be an R Markdown document. 

#### Information on the data

The data set is comprised of 651 randomly sampled movies produced and released before 2016.

Some of these variables are only there for informational purposes and do not make any sense to include in a statistical analysis. It is up to you to decide which variables are meaningful and which should be omitted. For example information in the the `actor1` through `actor5` variables was used to determine whether the movie casts an actor or actress who won a best actor or actress Oscar.

You might also choose to omit certain observations or restructure some of the variables to make them suitable for answering your research questions.

When you are fitting a model you should also be careful about collinearity, as some of these variables may be dependent on each other.

Source of information: Rotten Tomatoes (https://www.rottentomatoes.com) and IMDB (http://www.imdb.com) APIs.

#### Information on model selection

You may choose to use any of the Bayesian model selection techniques presented in this course, however you should justify your choice. Note that there are many other model selection techniques that are beyond the scope of this course, and those should not be used in this project.

Note that you have a very specific task on hand: predict audience_score based on the explanatory variables listed above. Also note that you first need to create some of these explanatory variables based on existing variables in the dataset.
