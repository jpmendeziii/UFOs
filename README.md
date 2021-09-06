# UFOs
## Overview of Project
### Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape.

* Deliverable 1: Filter UFO sightings on multiple criteria
* Deliverable 2: A written report on the UFO analysis README.md.

## Deliverable 1:
Filter UFO sightings on multiple criteria:
To start the update of the enhanced UFO website for the challenge, the index.html file had to be updated by removing the list element that creates the button.  Four more list elements were created: city, state, country, and shape. These will be like the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.  Please see image below.

![Resources/Challenge_Index_update_4_added_elements.jpg](Resources/Challenge_Index_update_4_added_elements.jpg)

In Step 1 of the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. Next, code was written for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().  In Step 3, a function was provided, updateFilters(). Inside this function, the code was written for Steps 4-5 to update the filters based on user input.  In Step 5, an if-else statement was written that checks if a value was changed by the user (variable from Step 4b). If a value was changed, add the element’s id (variable from Step 4c) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.  In Step 6, inside the updateFilters() function, call the filterTable() function that will be used in Step 7.  In the filterTable() function in Step 7, the code was updated to filter the table based on the user input that is stored in the filters variable.  In Step 8, a variable was created for the filtered data that is equal to the data that builds the table. This variable holds the updated table data based on the user input.  In Step 9, loop through the filters object and store the data that matches the filter values in the variable created in Step 8.  In Step 10, the table was rebuilt with the filtered data by passing the variable created in Step 8.  Please see image of code below.

![Resources/Challenge_Code_for_steps1_10.jpg](Resources/Challenge_Code_for_steps1_10.jpg)

For Step 2, located before the buildTable(tableData) function at the end of the starter code, the event listener was modified from this module so that it detects a "change" on each input element and calls the updateFilters() function.  Please see excerpt below.
![Resources/Challenge_Code_for_step2.jpg](Resources/Challenge_Code_for_step2.jpg)

When you start the index.html page, the resulting output is shown below.
![Resources/Challenge_Completed_Page_OUTPUT.jpg](Resources/Challenge_Completed_Page_OUTPUT.jpg)

To utilize the functionality of the UFO website, enter filter search criteria.  In this example, the shape "triangle" was entered and the output is shown below.  Also, to clear the search and restart, click the "Clear Table" button.
![Resources/Challenge_Completed_Filtered_Search_Triangle.jpg](Resources/Challenge_Completed_Filtered_Search_Triangle.jpg)
