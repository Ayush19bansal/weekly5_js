# Hosted link https://ayush19bansal.github.io/weekly5_js/

 This code appears to be a JavaScript code snippet for a web application that performs the following actions:

1. **Search Functionality**:
   - The `Search` function takes an `isShowAll` parameter, indicating whether to show all results or not.
   - It retrieves the search text from an input field with the id "searchField."
   - Calls the `loadPhone` function to fetch phone data based on the search text and shows a loading indicator during the request.

2. **Loading Indicator**:
   - The `loading` function toggles the visibility of a loading indicator with the id "loading" based on the `isLoading` parameter.

3. **Fetching Phone Data**:
   - The `loadPhone` function fetches phone data from an API using the provided search text.
   - Parses the JSON response.
   - Calls the `displayPhones` function to display the phone cards.

4. **Displaying Phone Cards**:
   - The `displayPhones` function takes an array of phone data and a boolean `isShowAll` to determine if all results should be displayed.
   - It updates the UI by generating and displaying phone cards.
   - If there are more than 12 results and `isShowAll` is false, it shows a "Show All" button.
   - It limits the number of displayed results to 12 if `isShowAll` is false.
   - Generates a card for each phone with details such as image, name, and a "Show Details" button.

5. **"Show All" Button**:
   - The `showBtn` function is called when the "Show All" button is clicked. It calls the `Search` function with `isShowAll` set to true to display all results.

6. **Showing Phone Details**:
   - The `showDetailsHandler` function fetches detailed information about a phone based on its ID.
   - Parses the JSON response and calls `showPhoneDetails` to display the details in a modal.

7. **Displaying Phone Details**:
   - The `showPhoneDetails` function updates the UI to show the details of a phone in a modal.
   - It sets the image, phone name, brand, specifications, and release date in the modal.

