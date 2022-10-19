# Project-3
An analysis of the TMDb movie data. Answering questions such as, most popular movie genres.

##Dataset
In this data set, there is a collection of 10,000 movies collected from the TMDb website. The data set has 10,796 rows and 15 columns. The columns consists of the id, tmdb id, popularity, budget, revenue, original title, cast, homepage, director, tagline, keywords, overview, runtime, genres, production companies, release date, vote count, vote average, release year as well as budget and revenue adjusted for inflation from 2010. 


##Wrangling Data
After loading in the dataset the data was wrangled to determine the number of columns and was further investigated usinng the info and describe function. After checking for duplicates and finding one, some columns that would not be investigated immediately were dropped. The adjusted budget and adjusted revenue, 'budget_adj' and 'revenue_adj' respectively was changed from exponential form to an int form.

##Cleaning Data
The genre column was separated seperated by the pipe(|) and using the .assign() and .explode()function into individual entries.

##Exploratory Data Analysis
To better explore the first question posed, the mean of popularity grouped by the genre was 
found and analysed in a bar plot and a scatter plot. Also, the mean of the vote count of 
various movies was analysed along with the popularity.
To better explore the second question, the mean adjusted revenue and genre were compared 
in a scatter and bar plot. Patterns of the adjusted revenue and release year were also evaluated 
to find which properties are associated with higher revenue.


##Findings
- Which genres have been the most popular?
In conclusion, three main genres that seem to be the most popular as well as have the 
highest vote counts were found. These three genres were Adventure, Fantasy and Science Fiction. The 
mean as well as the bar and scatter plots showed these patterns.
- Which properties are associated with higher revenue?
In conclusion, the most popular movie genres seem to be related to the movies that make the 
most revenue, shown in the bar and scatter plots. The years the movies were released show 
more revenue in a scatter plot. However, older movies have no information on their revenue 
and so this might be the reason for this reading from the scatter plot.
