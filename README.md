# library-management.
This project implements a simple Library Management page using HTML, CSS (Bootstrap), and JavaScript. It allows users to search for books by title and displays the search results dynamically.

Instructions:
HTML Setup
Add an HTML input element with id="searchInput" inside a container element.
Add an HTML container element with id="searchResults" to display the search results.

Functionality:
When a value is entered in the input element and the Enter key is pressed:
An HTTP GET request is made to the Books API with the query parameter title set to the value of the input element.
A loader (Bootstrap spinner) is displayed while fetching the data.
After the data is fetched, the search results are displayed in the searchResults element.
If the search results are empty, display "No results found" in the searchResults element.
If there are search results, append each result item to the searchResults element. Each result item should include:
An HTML image element with the src attribute set to the value of the imageLink from the HTTP response.
An HTML paragraph element with the text content set to the value of the author from the HTTP response.

HTTP Requests & Responses:
Books URL: https://apis.ccbp.in/book-store
Example URL: https://apis.ccbp.in/book-store?title=India
Query Parameter:
title: Value of the searchInput element. Example: India
Method: GET
Description: Returns a response containing the list of books with the title provided in the searchInput element.
