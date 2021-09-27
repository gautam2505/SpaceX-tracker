Steps to run the app:

# Install dependencies (server & client)
npm install
cd client && npm install

# Run server & client (:3000 & :5000)
npm run dev

# Server only (:5000)
npm run server

# Client only (:3000)
npm run client

# Build for production (Builds into server ./public)
cd client && npm run build

# Graphiql - http://localhost:5000/graphql


Visualizing the Project: The idea here is that app will log the details of all the launches executed by SpaceX, wherein the launch details are being fetched from the SpaceX graphql api endpoint. Once retrieved successfully, the client-side code is such that it will render a list of all the launches.

Although the client could have separate routes for the successful and the failed launches, but I have gone with a single page. And regarding the UI, as how to determine the success and the failure case, I have used some basic styling and marked up the Launch name in specific. For e.g. the launch name text in the list will be shown wit Green color for the successful launch and red for the failed launch.

Also, I have a specific route, to get to know more about the launch details, which can be accessed by clicking the LaucnDetails button.
