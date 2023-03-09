# mars-datascrape
Data scraping with BeautifulSoup in Jupyter Notebook delivers news articles about Mars and planet weather data

## Part 1: Scrape Titles and Preview Text from Mars News

The Jupyter Notebook part_1_mars_news.ipynb visits a static site on Mars news and scrapes the site for article titles and the preview text for each article with Beautiful Soup. The list of this information is printed in the Jupyter Notebook.

## Part 2: Scrape and Analyze Mars Weather Data

The Jupyter Notebook part_2_mars_weather.ipynb visits the Mars Temperature Data Site (a static website) and scrapes the tables there with Beautiful Soup. This data is assembled into a Pandas DataFrame. The column headings are:
<ul>
    <li><strong>id:</strong> the identification number of a single transmission from the Curiosity rover</li>
    <li><strong>terrestrial_date:</strong> the date on Earth</li>
    <li><strong>sol:</strong> the number of elapsed sols (Martian days) since Curiosity landed on Mars</li>
    <li><strong>ls:</strong> the solar longitude</li>
    <li><strong>month:</strong> the Martian month</li>
    <li><strong>min_temp:</strong> the minimum temperature, in Celsius, of a single Martian day (sol)</li>
    <li><strong>pressure:</strong> The atmospheric pressure at Curiosity's location</li>
</ul>

Data is converted to the appropriate datetime, int, or float data types. The data is analyzed to answer the following questions:

<ul>
    <li>How many months exist on Mars?</li>
    <li>How many Martian (and not Earth) days worth of data exist in the scraped dataset?</li>
    <li>What are the coldest and the warmest months on Mars (at the location of Curiosity)? The results are plotted as a bar chart.</li>
    <li>Which months have the lowest and the highest atmospheric pressure on Mars? This is plotted as a bar chart.</li>
    <li>About how many terrestrial (Earth) days exist in a Martian year? This answer is found by analyzing a line chart.</li>
</ul>

The data in the DataFrame is exported to a CSV file in the output folder.
