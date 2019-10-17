# Ford GoBikes Data Exploration
## by Reema Mohsin


## Dataset

This data consists of 1,863,721 individual bikes rides in 2018 using the Ford GoBikes bike-sharing system. The information on the bike ride includes start time, duration, bike id, user type, and much more. The data was collected [here] (https://www.lyft.com/bikes/bay-wheels/system-data). 


## Summary of Findings

In the data exploration, I looked at four main variables: duration, start time, user type, and member gender. Duration was originally given in seconds so I converted it to minutes through simple division to work with more readable numbers. I also used the start time to extract the start month specifically. The distribution of duration time was very heavily right-skewed so I transformed this column using a log scaling and found a unimodal distribution, with the most rides having a duration of between 5-10 minutes. I also found the trend of bike usage from month to month, with the summer months being higher in number of rides and the winter months being the lowest. Other variables I looked at were related to the user data, including type and gender. I found that a high majority of riders were Subscribers and males. There wasn't a specific relationship between month and duration of bike rides, but I did find that Customers on average take longer rides than Subscribers every month while Subscribers take more rides. In fact, subscribers account for 80% of all bike rides. This trend also persists within the gender category. Meaning even among males, females, and people of other gender, Subscribers have both a higher volume of rides while having shorter rides than Customers. When looking at gender alone, the duration time didn't seem to be relatively that different from month to month.

## Key Insights for Presentation

For the presentation, I focused on the three variables, duration time in minutes, month of ride start time, and user type to explain the trends and relationships in the 2018 data. I first looked at the distribution of each variable on its own, than plotted them against each other to see relationships between two variables at a time. Finally, I combined all three variables in one plot. Because two of the variables I looked at were categorical and the third was numerical, I used bar charts and Facet grids of boxplots or histograms to visualize the data. 

## Running the Slideshow

To remove code cells from slides, enter the following code into the command line:
`jupyter nbconvert "exploration_fordgobikes2.ipynb" --to slides --post serve --template output_toggle`
