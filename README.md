# Data_Collection_Module_11

## Part 1: Scrape Titles and Preview Text from Mars News

1. Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

      (a) Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview.

      (b) Store all the dictionaries in a Python list.

      (c) Print the list in your notebook.

### Output of query
 ![Alt text](/Images/Part_1_Result.PNG)

## Part 2: Scrape and Analyze Mars Weather Data

1. Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
      1. **id**: the identification number of a single transmission from the Curiosity rover
      2. **terrestrial_date**: the date on Earth
      3. **sol**: the number of elapsed sols (Martian days) since Curiosity landed on Mars
      4. **ls**: the solar longitude
      5. **month**: the Martian month
      6. **min_temp**: the minimum temperature, in Celsius, of a single Martian day (sol)
      7. **pressure**: The atmospheric pressure at Curiosity's location
  
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5. Analyze your dataset by using Pandas functions to answer the following questions:

   1. How many months exist on Mars? **Ans:12 Months**
        
   2. How many Martian (and not Earth) days worth of data exist in the scraped dataset? **Ans:1866**
        
   3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
               
      1. Find the average minimum daily temperature for all of the months.
      2. Plot the results as a bar chart.
      3.  ![Alt text](/Images/Average_Temp_Ploting.png)
     
   4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
      
      1. Find the average daily atmospheric pressure of all the months.
      2. Plot the results as a bar chart.
      3. ![Alt text](/Images/Average_Pressure_Ploting.png)

   5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:

      1. Consider how many days elapse on Earth in the time that Mars circles the Sun once.
      2. Visually estimate the result by plotting the daily minimum temperature.
      3.  ![Alt text](/Images/Earth_Days.png)
     
  6. Export the DataFrame to a CSV file.
   
     
