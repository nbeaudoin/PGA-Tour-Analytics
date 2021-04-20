# PGA-Tour-Analytics
Analysis of PGA Tour from 1980 to present day

# Get Stat ID script
This script returns all the statistic IDs tracked by PGATour.com. Unless you think there is a new stat added, then this script only needs to be run once.

# Tournament Names script
Each time you want to scrape a statistic, you need to enter in the ID number and category into this script. The script returns all the tournaments that the respective stat ID has information on. These tournament names are fed into the statistic scrape script.

# Scrape Job script
This script scrapes statistics for each tournameny by each year. It takes in the Tournament Name script that the user ran for the specified stat ID. You will need to enter the category of the statistic (ie, "Off the tee") and the stat ID of the statistic you wish to scrape. The output file will check if the statistic has been run before, avoiding additional compute time. If it has, then it is not added, but if it is not in the output csv, then it is added. This can be run after each tournament week.