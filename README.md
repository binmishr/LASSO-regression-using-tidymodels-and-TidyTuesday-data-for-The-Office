# LASSO-regression-using-tidymodels-and-TidyTuesday-data-for-The-Office

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.


The Office - Words and Numbers
=================================
The data this week comes from the schrute R package for The Office transcripts and data.world for IMDB ratings of each episode.

If you'd like to use the schrute R package for ALL the lines/dialogue from the show - please install it from CRAN via install.packages("schrute"). A quick example from the vignette can be found here.If you want to do text analysis - make sure to check out the tidytext package - a vignette can be found here and the Tidy Text Mining with R book can be found freely online here.

Lastly - the pudding analyzed The Office dialogue across a few charts 

Get the data here
# Get the Data

office_ratings <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-03-17/office_ratings.csv')

# PLEASE NOTE TO USE 2020 DATA YOU NEED TO USE tidytuesdayR version ? from GitHub

# Either ISO-8601 date or year/week works!

tuesdata <- tidytuesdayR::tt_load('2020-03-17')
tuesdata <- tidytuesdayR::tt_load(2020, week = 12)
office_ratings <- tuesdata$office_ratings
