# Project1

Milestone 1

September 24, 2024

Project Idea

Our project idea looks at comparing movie streaming trends for movies found on pirated and streaming platforms, specifically analyzing features such as movie rating, genre and number of watches, content accessibility and pricing, to identify any trends in consumption patterns between the two that may shift usage or behavior in user preferences when watching movies.
Member Contributions

Maïté Sadeh:
Brainstormed various initial ideas, created and shared google drive folder, helped edit final project idea statement

Matthew Sadowski:
Brainstorming idea, shared document, found movie piracy dataset that we may potentially use.

Benjamin Perl:
Brainstormed topics
Drafted project descriptions

Kai Barker:
Topic brainstorming, dataset collection, drafted description and piracy idea


Milestone 2
October 1st, 2024
Progress
We have searched for and procured new datasets based on milestone 1 feedback, refined channels for analysis, and initialized the group GitHub repository with a Readme and dataset uploads. Work has started on drafting visualizations and some initial data cleaning and tidying.
Member Contributions
Maïté Sadeh
Searched for new datasets
Refined channels for analysis 
Matthew Sadowski
Initialized group Github repository (Readme, uploaded datasets, etc)
Drafted visualizations
Benjamin Perl
Procured new datasets based on milestone 1 feedback
Started on some data cleaning/tidying
Compiled Milestone 2 write up
Kai Barker
Drafted visualizations
Searched for new datasets
Refined channels for analysis 

Comparing Different Streaming Services Show Ratings vs. Their Prices
Kai Barker, Benjamin Perl, Maïté Sadeh, Matthew Sadowski




Description of the Data:

For this project, we used two different datasets obtained from Kaggle. The first dataset reported on different movies on streaming platforms: Netflix, Hulu, Prime Video, and Disney+., and recorded the Rotten Tomatoes scores for the movie. Variables included the movie title, year the movie was released, age appropriateness of the movie, Rotten Tomatoes score (represented as a number out of 100), and columns for each streaming platform with values of 0 (no) or 1 (yes) to indicate whether or not the movie is shown on the given platform. Variables such as movie title, movie release year, and age appropriateness were unnecessary that were not included in the development of the visualizations. 

The second dataset we used included the prices of the streaming platforms for Netflix, Disney+, HBO Max, Hulu, Paramount+, Prime Video, Apple TV+, Peacock, Shudder, and Crunchyroll, spanning a time period from 2011 to 2024. The variables were the service name, date for given service price at that time in the format of mmm-YYYY (ex. Jan-2024), and the price. Given that the first dataset only reported on movies from four streaming platforms (Netflix, Hulu, Prime Video, and Disney+), we did not have to include the other streaming service prices when rendering our price bar graph.

From the first movie dataset, the Rotten Tomatoes score had to be transformed into an int from its original form of a fraction since we had to do math on the values later on for the box plot. In addition, the variable that indicated whether or not the movie was shown on a service was represented in binary. The rotten tomatoes score had to be mapped to the service it was shown on to be able to represent the scores across the streaming platforms. As we were only looking at the Rotten Tomatoes scores with relation to the streaming platforms and their prices, any variables that were not related to this were able to be discarded.

Design Rationale Overview:

In our visualizations, we wanted to make sure that the color scheme we chose matched the colors of the corresponding logos that the data represented (i.e. red for Netflix, green for Hulu, etc.) This was important because it would make it easier for viewers to immediately match the data with the appropriate streaming service it represented with minimal effort. We slightly altered Disney's color to be a lighter shade of the blue logo as the original color made it harder to view. We also made the circles that represented the Rotten Tomatoes data points have an opacity so that it wouldn’t clash with the boxplot over it. It is helpful extra information but not the main focus of that particular graph visualization, which is also why we put the plotted points behind the box plot so it wouldn’t distract too much. For the bar plot, we included logos and the corresponding colors for each rectangular bar so that it would be more easily distinguishable. Both visualizations placed the streaming services in the same order side by side on the horizontal x-axis so it would be easily comparable.

We also performed linear scales on the y-axis and scale band on the x-axis for the box plot. In the bar plot, the y-axis starts at $10 instead of 0 like the scale that the box plot graph takes. This is because the lowest starting subscription price per month out of all four platforms is $12 for Prime Video. We did not believe it necessary to start at $0 because otherwise there would be a lot of space being used and the length of the bars would be too long and make the visualization less readable. This way, viewers are still able to tell which platforms are more expensive than others without compromising the integrity of the data. It is also ok that it is not the same scale as the box plot since one is a box plot and the other is a bar graph so it wouldn’t affect the analysis.

Visualization Story:

Through the two visualizations we displayed––the box plot for the rotten tomatoes scores across streaming platforms, and the bar chart indicating the price per month for the four streaming services––we aimed to find relationships between the strength of a given streaming platform and their corresponding price. It is interesting to note that there is a cluster of scores for the Netflix streaming service in between the bottom of the box plot and the lower outlier. This is around the same value of the lowest outliers marked on the other three services. Most likely, most movies aren’t rated with Rotten Tomatoes scores below ~10%, except for the outliers with Netflix. In addition, we found that Hulu had the highest mean for the Rotten Tomatoes score, as well as the highest monthly subscription price, whereas Prime Video had both the lowest mean score and subscription price. 

Prime Video also had less outliers as seen from the box plot whiskers, but Netflix had the largest variation in output values with outliers ranging from Rotten Tomatoes scores of 0 to almost 100. Originally, we thought that this could be due to the sheer volume of title offerings Netflix has, which could explain the variation of Rotten Tomatoes scores. However, upon further research, we found that Prime Video has more title offerings at ~18,002 compared to Netflix’s offerings of ~6,855 titles (https://qz.com/streaming-services-content-library-netflix-disney-hulu-1851540874/slides/9). Another reason for this could potentially be because Netflix has a larger viewership than Prime Video, boasting 247 million subscribers compared to 200 million subscribers respectively (https://www.voronoiapp.com/entertainment/Top-Video-Streaming-Platforms-By-Number-of-Subscribers-579). With a larger audience also comes more variance with the types of offerings to cater to the different audiences, which may therefore affect the quality of the offerings. However, the low mean and overall low scores for Prime Video suggest that the platform does not have as good options as the other platforms, and Netflix just happens to have more outliers.

Another observation that could be made from the graphs was that Disney+ had better Rotten Tomatoes scores overall (mean, min, max values shown on the box) compared to other services like Netflix but Netflix has a more expensive subscription price than Disney+. This result was surprising since Netflix is more widely talked about and used compared to Disney+. An explanation to this perhaps could be that Disney+ has a smaller catalog, that is very narrow and specific to a particular target audience. There is less room for variance, and the offerings they do have include a very loyal fanbase (such as the Marvel and Star Wars movies) contributing to higher Rotten Tomatoes scores.

Overall, there was a lot of insight that could be gleaned from our visualizations, and it was very interesting to see how the pricing and Rotten Tomatoes scores compared across all four platforms we analyzed.



Team Contributions:

Kai Barker:
Helped work on the barplot (1 hr), drafted final directions (1hr), and created and polished the final visualizations. (2.5 hours)

Benjamin Perl:
Helped work on the barplot (1hr), contributed to new direction planning (1hr), and other initial and final visualizations (1hr)

Maïté Sadeh:
Did the write up for the final report (about 1.5 hrs), contributed to final aesthetic enhancements and visualizations (about 2 hrs)

Matthew Sadowski:
Created a github repo, did the first draft of a visualization (about 1 hr), and we eventually went in another direction with our data. Created the first version of the boxplot with our new data, added some graph titles (about 2 hrs).

Time Breakdown:

Development was done in sections and ran fairly smoothly. The part of the project that took the most time was ideation, and identifying areas in which we could improve our base visualizations. After we agreed on extra finishes to add to our base graphs (logos, point inclusion, color matching, etc.) our implementation did not take a long time.





