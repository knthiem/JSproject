Final Project for Internet II by Kenny Nanthavong


Index page
-------------------

A page to simply present the project

Module 1 & 2
-------------------

These modules make use of array iteration and AJAX request that returns JSON objects.
The API used is the New York Times API to search for movie reviews.

The text bar allows user to input any string. The search button calls a function to make a request to the New York Times API making use
of the user input as an option to the request. The API returns a response in JSON an the response is stored in an array of objects. That same
function then calls another function to generate a string that contains the html needed. To generate the html the forEach() iterator is used to 
go through the array to get the data needed. The string is then used to output the search result in a table.

Another button is to search reviews from the last 7 days. Upon clicking the button, a function similar to the first function is called, except a parameter 
is added to search between specified dates. Using the date object, it is possible to find today's date and the date from 7 days ago. The array iterator
used in this function is the reduce() iterator to generate the html output.

The last button is used to display reviews published on the current day. Making use of the same function as the first one and using the date object to
get the current date, the filter() iterator is used on the resulting array of the AJAX request to make a new array that keeps only the objects needed.
The html is then generated to show the result to the user.

Module 3
-------------------

This module make use of Chart.js.

A line chart is first shown with no data. The chart's Y axis is for the weight in kilogram and the X axis is for the 12 months. The user can selected a month
in the dropdown list and only input a number of the input bar. Once the user clicks the add button, the chart will be updated with the approriate data.

The function used to update the data first checks the index of the element chosen in the list. Next, the data in the chart object is modified with user input from
the number input bar. As the data is stored in an array, the index will be used to know which element to modify in the array. Chart.js then has a function called
update() to output the result of the added data in the chart.

References
-------------------

 jQuery.ajax
http://api.jquery.com/jquery.ajax/

New York Times API
https://developer.nytimes.com/

Bootstrap
https://getbootstrap.com/docs/4.1/getting-started/introduction/

Chart.js
http://www.chartjs.org/docs/latest/