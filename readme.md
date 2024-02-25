The oldest programming language is Assembly, a language that was still being taught at the school I attended (a clear example of how public education keeps up with technology or current affairs in general  😂 ). I remember they stopped teaching it just as we reached the last three years of school, replacing it with C++... Anyway, from the 1940s, when Assembly was the only language, until now, I would say a lot has changed. Now there are as many languages as there are branches of employment... But which programming language is the most popular? the one people just can't stop talking about? The rockstar of languages, or how has the popularity of certain languages changed over the years.

StackOverflow will help us answer this burning question. Each post on Stack OverFlow comes with a Tag. And this Tag can be the name of a programming language.To figure out which language is the most popular, all we need to do is count the number of posts on Stack Overflow that are tagged with each language. The language with the most posts wins!

￼

In this notebook I have seen how to grab some raw data and create some interesting charts using Pandas and Matplotlib. I have:
▪  used .groupby() to explore the number of posts and entries per programming language
▪ converted strings to Datetime objects with to_datetime() for easier plotting
▪ reshaped the DataFrame by converting categories to columns using .pivot()
▪ used .count() and isna().values.any() to look for NaN values in the DataFrame, which I then replaced using .fillna()
▪ created (multiple) line charts using .plot() with a for-loop
▪ styled the charts by changing the size, the labels, and the upper and lower bounds of the axis.
▪ added a legend to tell apart which line is which by colour
▪ smoothed out the time-series observations with .rolling().mean() and plotted them to better identify trends over time.


Through this page tackexchange ( https://data.stackexchange.com/stackoverflow/query/675441/popular-programming-languages-per-over-time-eversql-com ), it is possible to launch a query and download a CSV file of the posts published on StackOverflow.

The CSV file that I downloaded and worked on has 2580 rows and 3 columns. I renamed the columns in order to give them meaning and work more easily.

￼
Using the groupby() function, I sum up the posts with the same tag and save the resulting list in a variable. Later, I sort this variable and set the 'ascending' parameter to 'False' (since by default it's set to 'True'). This allows me to have the sum values in descending order, so the programming language with the highest number of posts will be at the top of the list, followed by those with fewer posts until the language with the lowest number of posts.

￼

____________

My comment is limited to what I could see based on this data, based on the number of posts published on StackOverflow and grouped according to their respective tags (referring to programming languages) from 2008 to February 2024...
Once I cleaned the data and a projection of the post numbers per month for all languages was created on a timeline, I could clearly see the trend of various languages. For example, which language was the most popular during the x/y timeframe, which one had the fewest posts in a particular timeframe, which languages are the oldest, most recent, etc

￼
