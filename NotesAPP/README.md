 FastAPI Notes App Documentation
📌 Overview
The FastAPI Notes App is a simple web-based application that allows users to add, view, and store notes in a MongoDB database. It provides a web interface where users can interact with the notes system and stores all data in a cloud-based MongoDB database.

🛠️ Tech Stack
Backend: FastAPI (Python)
Database: MongoDB (Cloud via MongoDB Atlas)
Frontend: HTML + Bootstrap
Templating Engine: Jinja2
Web Server: Uvicorn
📂 Project Structure
config/ → Contains database configuration files.
models/ → Defines the data models using Pydantic for validation.
routes/ → Contains API route definitions for handling user requests.
schemas/ → Converts MongoDB documents into JSON-compatible format.
static/ → Stores static assets such as CSS and JavaScript.
templates/ → Contains HTML templates for rendering pages.
index.py → The main FastAPI application file.
requirements.txt → Lists dependencies required to run the project.
🚀 Installation and Setup
1️⃣ Clone the Repository
Download or clone the repository to your local machine.

2️⃣ Install Dependencies
Install the required Python libraries from the requirements.txt file.

3️⃣ Configure MongoDB Connection
Update the MongoDB connection string inside the database configuration file.

4️⃣ Run the Application
Start the FastAPI application using Uvicorn, which will serve the web interface and API.

🛠️ API Endpoints
GET / → Fetches and displays all stored notes in the web interface.
POST / → Allows users to submit new notes, which are stored in MongoDB.
DELETE /{id} → (To be implemented) Deletes a specific note from the database.
📜 Project Workflow
The user visits the homepage, where existing notes are displayed.
The application fetches stored notes from MongoDB and renders them on the webpage.
Users can add new notes by submitting a form.
Submitted data is sent via an API request and stored in MongoDB.
The page refreshes to show the newly added notes.
