# npx-create-react-app-map-app

Objective: This assignment aims to evaluate a candidate's ability to develop a React application incorporating a map using an open-source library, implementing secure authentication, and creating a visually appealing user interface. The goal is to assess the candidate's proficiency in React, API design, authentication techniques, UI/UX principles, and overall code quality. Expected learning outcomes include practical application of React concepts, understanding of authentication methods, experience with map integration, and an appreciation for UI/UX design considerations.

Step-by-Step Instructions:

Project Setup and Initialization:

Create a new React project using Create React App or a similar tool.
Navigate to the project directory in the command line.
Install the necessary dependencies, including React Router, an open-source mapping library (e.g., Leaflet or OpenLayers), a library for making API requests (e.g., Axios or Fetch), and any styling libraries (e.g., Material UI, Bootstrap, or Styled Components).
Development Process:

Backend API Development:
Set up a Node.js backend with Express to handle API requests.
Implement the following API endpoints:
Login API: Create an endpoint (/api/login) that accepts user credentials (username and password) and authenticates the user. Implement a robust authentication mechanism (e.g., JWT - JSON Web Tokens).
Dashboard API: Create an endpoint (/api/dashboard) that returns data for the dashboard, including card component information. This endpoint should be protected and only accessible to logged-in users.
Map View API: Create an endpoint (/api/map) that returns necessary data for the map view, such as the initial map center coordinates, zoom level, or other relevant map configurations. This endpoint should also be protected.
Implement error handling to return appropriate messages (e.g., "User not logged in") when a user is not authenticated.
Authentication Implementation:
Implement a JWT-based authentication system.
Upon successful login, generate a JWT token and send it to the client.
Store the JWT token in the client (e.g., using local storage or cookies).
Include the JWT token in the headers of subsequent API requests to authenticate the user.
On the backend, verify the JWT token on protected routes before processing the request.
React Frontend Development:
Create React components for the following:
Login Page: Design a user interface for the login page with input fields for username and password, and a submit button.
Dashboard: Create a dashboard component that displays card components. Each card should have a unique ID.
Map View: Create a map view component that displays the map of India using the chosen open-source mapping library.
Implement routing using React Router to navigate between the login page, dashboard, and map view.
Implement the logic for handling user login and storing the JWT token.
Implement the logic for making API requests to fetch data for the dashboard and map view.
Implement the logic for redirecting the user to the dashboard if they are logged in.
Implement the logic for displaying the "User not logged in" message if the user is not authenticated and tries to access the dashboard or map view.
Implement the logic for zooming in and zooming out on the map.
Map Integration:
Integrate the chosen open-source mapping library (Leaflet or OpenLayers) into the Map View component.
Display the map of India.
Set the initial zoom level to show a zoomed-out view of India.
Implement zoom in and zoom out functionality using the mapping library's API.
Component Interaction:
When a card component on the dashboard is clicked, navigate the user to the Map View component.
Pass the unique ID of the card component to the Map View component (optional - if the card ID is relevant to the map view).
Styling and Design:

Implement the UI design for the login page, dashboard, and map view.
Use CSS, a CSS framework (e.g., Material UI, Bootstrap), or a CSS-in-JS library (e.g., Styled Components) to style the components.
Ensure the UI is visually appealing, responsive, and user-friendly.
Pay attention to UI/UX principles, such as color scheme, typography, and layout.
Refer to the Figma portfolio for design inspiration and consistency.
Deployment:

Choose a suitable platform for deploying the backend API (e.g., Heroku, AWS, or Google Cloud).
Deploy the backend API to the chosen platform.
Choose a platform for deploying the React frontend (e.g., Netlify, Vercel, or AWS S3).
Configure the React frontend to point to the deployed backend API.
Deploy the React frontend to the chosen platform.
Submission Guidelines:

Submit the entire project code, including the React frontend and the Node.js backend.
Include a README.md file with clear instructions on how to set up and run the project.
Document all the packages used in the project and explain their purpose.
Include the link to your Figma portfolio in the README.md file.
Ensure the code is well-organized, readable, and follows coding standards.
Submit the assignment as a ZIP file or a link to a Git repository.
