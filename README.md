# Goal
- In this challenge, I was tasked with completing a full web-scraping and data analysis project
- I was provided with two websites on the topic of the planet Mars, one consisting of news articles and the other a table of weather data
- Part 1 of the project was to scrape tiles and preview text from news articles
- Part 2 was to scrape and analyze Mars weather data

# Method
- Part 1 - Scraping Tiles
   - To complete this task, I pointed the local browswer to the provided website with news      articles regarding Mars
   - I created a Beautiful Soup object, extracted the text elements including article titles    and teasers, storing them in a list
   - I then converted the list to a Pandas DataFrame and wrote the results to a JSON file     for ease of sharing the data
- Part 2 - Scrape and Analyze Table
   - To complete this task, I pointed the browser to the website containing the table of        Mars temperature data, created the Beautiful Soup object, and extracted the rows of data
   - The data was stored into a list by row
   - I then created a Pandas DataFrame with the same headers as the html table to store the    data
   - The datatypes of the rows was updated for easier analysis
   - Using this DataFrame, I anaylized the data to answer the questions (e.g. how many          Martian months are included in the dataset [12], how many Martian days [1867], the          minimum average temperature and atmosphering pressure by month, etc.)
   - The results were printed to the notebook, converted to DataFrames, and plotted
   
# Summary and Results
- The JSON file containing the resulting data from Part 1 of the challenge can be found in the Output folder entitled Mars_News.json
- For Part 2, I plotted the temperature DataFrame to demonstrate the trend:

![image](https://user-images.githubusercontent.com/120341249/225492335-bab8d3f6-9b8a-402e-9082-65fb08878f8a.png)

   - I confirmed the 3rd Martian months is on average the coldest (-83.31 C), while the      8th is on average the warmest (-68.38 C)
   - I then plotted the pressure DataFrame:

![image](https://user-images.githubusercontent.com/120341249/225492521-f5d74c25-b4ae-49f2-8c2d-9718e6525d88.png)

   - I confirmed the 6th month has the lowest average atmospheric pressure (745.05) while    the 9th has the highest (913.31)

   - I then plotted the DataFrame showing the daily minimum temp:

![image](https://user-images.githubusercontent.com/120341249/225492748-36d6d032-4719-486b-9f9f-fbfb7c009564.png)

   - Using this plot and sorting the results to find the temperature "peaks" to represent    one year roughly, I estimated there are 672 terrestrial (Earth) days in a Martian year
   - I then confirmed at mars.nasa.gov that there are actually 687 Earth days in a          Martian year 
   - The initial DataFrame and all plots were saved and can be found in the Output folder    of this repostory (Month_Temp.png, Pressure.png, Daily_Temp.png, and Mars_Data.csv)
