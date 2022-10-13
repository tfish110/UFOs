# UFOs
## Overview

This project's goal was to help Dana build a webpage to display table data on UFO sightings. I was tasked with modifying the HTML code for the webpage to have multiple text entry boxes to filter the table by various parameters. I then had to write a script to handle the filter requests that a user might enter and update the table to reflect the filtered results.

### Resources
- Data: data.js, style.css
- Software: Visual Studio Code 1.70.1, Google Chrome 106.0.5249.103

## Results

![Filter Search](https://github.com/tfish110/UFOs/blob/main/Resources/filter_search.jpg)

Here, you can see the "Filter Search" section of the webpage where a user can enter text to filter the table by certain parameters. The filter options correspond to the headings of the first five columns of the table. In each box there is sample text which indicates the format that should be used for each search filter entry. For example, for the "State" search filter a user would enter "ma" rather than "Massachusetts" to search for UFO sightings in that state. Once the user types the desired search term, they can either press "Enter" or click outside the entry box and the table filter will execute.

![First Five Table Rows](https://github.com/tfish110/UFOs/blob/main/Resources/table_first_5.jpg)
![First Five Massachusetts Table Rows](https://github.com/tfish110/UFOs/blob/main/Resources/table_filtered_ma.jpg)

The first table shown here is the first five rows of the entire table as they appear when first loading the webpage. Using the "ma" state search filter example, the second table shown here displays the filtered table once the search filter is executed. To undo the filter, simply delete the search parameters that were entered, and the full table will display again.

![Multiple Filters Table](https://github.com/tfish110/UFOs/blob/main/Resources/table_filtered_date.jpg)

Finally, users can also filter on multiple parameters simultaneously, as shown here with the "ma" state search filter combined with a "1/7/2010" date search filter.

## Summary

This filter design does a good job narrowing the data to a more focused scope, but it could still be improved upon. One major draawback is that there is plenty of room for user error in this design. To search for UFO sightings in Massachusetts, you must enter "ma" in lowercase letters only. You cannot use the full name "Massachusetts", the capitalized abbreviation "MA" or any other string to get those results.

Among the improvments that could be made, changing the text entry forms to drop-down menus would limit the filter search terms to only those that would work to successfully filter the table. Another helpful tool might be to display a message if the filters selected yield no results, either as a result of there being no results in the data that match the desired parameters, or because of an error in the search term entered by the user. As it stands now, it simply displays a blank table instead.