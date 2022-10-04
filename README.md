# School_District_Analysis

## Project Overview
Maria is the chief data scientist for a city school district. Using Pandas, the standardized test and budget data from the city schools was cleaned up and aggragated to find any trends in school performance.

## Resources
- Data Source: new_full_student_data.csv
- Software: Python 3.7.6

## Summary

To perform the analysis, a five step process was done. 

    (1) First, the data supplied by Maria had to be imported and converted into a DataFrame. 

    (2) Second, the data needed to be cleaned. Upon inspection of the data, there were values that were NaN and there were duplicate rows. The rows with NaN were removed using the .dropna() function and 1,835 rows were removed using the .drop_duplicates() functions. It was also noted that the grade column was considered an object since upon inspection the grade numbers were amended with a "th". The text was eliminated and the column was converted to an integer in order to perform mathematical analysis on that column. 

    (3) Third was to summarize the data and the .describe() function was used to find the mean, standard deviation, minimum, first, second, and third quartiles, and the min and max. 

    (4) Fourth step was to drill down into the data using the .loc function to find and display desired rows. 

    (5) In the fifth step, the groupby() function was used to aggregate data for Charter and Public schools and the mean and count functions were used to make comparisons between the two. There were fifteen schools total in the data set and on average, the public schools got more funding. The math scores were compared between the charter and public schools per grade and it looks the math schools are higher for freshman and sophomore in charter schools but then they seem to trend downwards and are more on par with the math schools in the public schools for juniors and seniors. 

Other possible further analysis that can be done:
    (1) Determine the population of the high schools and group them by type to see if there is a higher population of students attending public school than charter schools or vice versa. This might shed light on as to why the public schools get more funding on average. 
    
    (2) It would also be advantageous to find the average reading score by grade for each school type alongside the reading score to see if that follows a similar or has a different trend. 