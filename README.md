## TCG Booster Pack Simulator Application Flask Design

### HTML Files

- `index.html`:
  - Main page of the application, serving as the entry point for users.
  - Contains the HTML form for selecting TCG, pack size, and other simulation parameters.
  - Includes the necessary JavaScript functions for handling form submission and displaying simulation results.
- `results.html`:
  - Displays the results of a simulated booster pack opening, including card images, descriptions, and statistical information.
- `collection.html`:
  - Allows users to view and manage their digital card collections, including import and export functionality.

### Routes

- `/`:
  - GET: Renders the `index.html` page with the form for simulation parameters.
  - POST: Receives the form data, generates a random card pack, and redirects to the `results.html` page with the simulation results.
- `/results`:
  - GET: Renders the `results.html` page with the generated card pack data.
- `/collection`:
  - GET: Renders the `collection.html` page with the user's card collection data.
- `/api/cards`:
  - GET: API endpoint for retrieving card data from the database.
- `/api/collections`:
  - POST: API endpoint for saving user card collections to the database.
- `/api/imports`:
  - POST: API endpoint for importing card collections from external sources.