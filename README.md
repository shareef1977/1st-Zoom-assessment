
# Project Title

A brief description of what this project does and who it's for


# Cameras API
This is a RESTful CRUD API for managing cameras and camera networks.
## Stack/Frameworks Used
• Node.js
• Express.js
• MongoDB
## API Endpoints
### Cameras
• GET /cameras: Get all cameras
• POST /cameras: Create a new camera
• PUT /cameras/:id: Update a camera by ID
• DELETE /cameras/:id: Delete a camera by ID
### Camera Networks
• GET /cameraNetworks: Get all camera networks with their cameras
• POST /cameraNetworks: Create a new camera network
• PUT /cameraNetworks/:id: Update a camera network by ID
• DELETE /cameraNetworks/:id: Delete a camera network by ID
## API Data
### Cameras
A camera object has the following properties:
• id: The ID of the camera (auto-generated by the database)
• name: The name of the camera (string)
• description: The description of the camera (string)
• url: The URL of the camera (string)
### Camera Networks
A camera network object has the following properties:
• id: The ID of the camera network (auto-generated by the database)
• name: The name of the camera network (string)
• description: The description of the camera network (string)
• cameras: An array of camera objects (array of objects with id, name, description, and url properties)
## API Responses
### Success Response
A successful API response has the following format:
{
  "status": 200,
  "data": ...
}

The data property contains the requested data (e.g., a camera object or an array of camera network objects).
### Error Response
An error API response has the following format:
{
  "status": 400,
  "error": ...
}

The error property contains an error message (string).
## Getting Started
1. Clone the repository
2. Install dependencies: npm install
3. Set up the database (e.g., create a cameras collection and a cameranetworks collection)
4. Set up the environment variables (e.g.,PORT and MONG_URI)
5. Start the server: npm start
