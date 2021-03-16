# Explore_Weather_Trends
Explore-Weather-Trends-Udacity-Data-Analysis-Nanodegree

# Exploring Weather Trends - Project Instructions
Summary
In this project, you will analyze local and global temperature data and compare the temperature trends where you live to overall global temperature trends.

# I. Steps taken to extract the data from SQL to be visualized in Excel:
1. Tools: Sql (Udacity Workspace version)
2. SELECT city FROM city_list WHERE country = 'Chile'
SELECT year, city, country, avg_temp FROM city_data WHERE city = 'Los Angeles' AND country = 'Chile'
SELECT avg_temp, year FROM global_data
3. Downloaded and saved it as Avg_temp_Los_Angeles_1855_2013.csv
4. Downloaded and saved it as Avg_temp_world_1750_2015.csv
5. Changed format from CSV to .xlsx of files; open both files.
6. Create two new columns world_five_year_mavg_temp (column C) and los_angeles_five_year_mavg_temp (column E)
7. Switching all the commas into dots, in order to avoid the zero division error.
8. Calculating the moving averages: Type in C6 =AVERAGE(B2 : B6); moving average from 1750 to 2015. Drag down the formula until the end of the data.
9. Calculating the moving averages: Type in E111 AVERAGE(D107:D111); moving averages from 1850 to 2013. Drag down the formula until the end of the data.
10. Line Chart: Creating a line chart by selecting the data and formatting it.
11. Key considerations:
- Chilean city Los Angeles has been selected because this city is the closest big city to where I live; Santiago, Chile.
- Moving averages have been computed based on a 5-yr convention; the five-year interval was selected because it smooths data out, while at the same time it keeps peaks and trends somewhat close to the original data. Compared to the 2-yr and the 10-yr moving averages, the 5-ys moving average provides a good balance between asymmetry and silkiness of the data.
- Since the data-set from Los Angeles starts in year 1850, this year has been selected as the starting point, even though the Global data-set begins in 1750.
- The Data set from Los Angeles only reaches up until 2013; however, year 2015 has been set as the ending point, because it corresponds with Global data-set ending year.
- Smoothed values have been computed from the fifth year on; that is why transparent lines and solid lines do not start at the same point.
