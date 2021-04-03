# TMDB Movies Dataset Analysis

[![LinkedIn][linkedin-shield]][linkedin-url]
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#key-questions">Key Questions</a>
    </li>
    <li>
    <a href="#new-set-of-questions">Updated Key Questions</a>
  </li>
 <li>
 <a href="#summary-of-findings">Summary of Findings</a>
 </li>
 <li>
 <a href="#limitations">Limitations</a>
 </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>


## About The Project
Dataset: TMDB Kaggle Dataset was selected for analysis. This dataset should help answer some interesting questions about movies. For each movie (row) in the dataset we have 21 features (columns) to describe it; such as Budget, Revenue, User Ratings, and other features.

## Key Questions

1) What is the relationship between Movie Budgets and the amount of Revenue they generate?

2) Does a higher budget translate into higher revenues?

3) What is the relationship between a movie's Budget and its Popularity?

4) What is the relationship between a movie's Runtime and Vote Average? Do longer movies receive lower ratings?

#### However, after realizing that data on Budget and Revenues is missing, a new set of questions was formulated. 

Data for missing Revenue and Budget are marked as 0.0 rather than NaN, and did not show up in early data inspection when running df.isnan() or df.info(). More than 50% of the data was 0.0 when running df.describe() which drew attention to the missing values. We can replace the missing data with the mean, but that wouldn't lead to an accurate analysis. Instead, a new set of questions is posed.

## New Set of Questions:

1) What is the relationship between a movie's Runtime and Vote Average? Do longer movies receive lower ratings?

2) Which movies were the most profitable?

3) Which movies earned the most amount of revenue?

4) Which year did we have the highest number of profitable movies?

6) What is the average runtime of all movies?

7) Who were the most frequently cast actors across all movies?

## Summary of Findings
The Average Runtime of all movies is 109.2 Minutes.

The Average Runtime of the top 100 profitable movies is 129.83 Minutes.

The Top 3 Most Profitable Movies were: Avatar, Star Wars: The Force Awakens, and Titanic.

The Top 3 Revenue Generating Movies were: Star Wars: The Force Awakens, Titanic, and The Avengers.

The Most Cast 5 Actors are: Robert De Niro, Bruce Willis, Samuel L Jackson, Nicolas Cage, and Matt Damon.

2015 is the year of highest profits for the entire dataset.

1966 is the year of least profits for entire dataset. Profits steadily increasing over time.

**Keep in mind: Correlation != causation.**


## Limitations
We have some missing values in the dataset affecting our results.

We don't know the currency used in the dataset.

Data for Budget and Revenues have a lot of 0. Had to deal with them.

Duplicates in the data skew results.

Incorrect datatypes had to be fixed

<!-- CONTACT -->
## Contact

Kareem Ayyad- [@kareem_ayyad](https://twitter.com/kareem_ayyad) - kareem@ayyad.net

Project Link: [https://github.com/KareemAyyad/TMDB-Analysis-Project-DAND](https://github.com/KareemAyyad/TMDB-Analysis-Project-DAND)

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/kareemayyad/
