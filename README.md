# FETCHED PROJECT - mcm group
Fetched is web application crafted to streamline the process of finding accommodations within the Veneto region. Beyond its primary function of aiding in accommodation searches, Fetched offers a rich array of supplementary features to enhance the visitor experience.

In addition to a diverse range of lodging options, Fetched acts as a valuable travel companion by furnishing users with insightful suggestions for nearby museums. This feature enables travelers to delve into the vibrant culture of the region, exploring its artistic heritage and historical significance.

Moreover, Fetched goes beyond mere lodging recommendations and museum insights. It paints a vivid portrait of the Veneto region by presenting captivating descriptions complemented by images for each of its provinces.

By seamlessly integrating accommodations, museum recommendations, and evocative snapshots of Veneto's provinces, Fetched provides users with an immersive exploration of this captivating Italian region.

# Flask and FastAPI Dockerized Project
This project demonstrates a simple web application using Flask as the frontend and FastAPI as the backend. The frontend allows to search for a city in Veneto and the result is given by the backend using a search bar.

The project is Dockerized for easy deployment.

## Architecture
The project follows a simple client-server architecture:

1. **Frontend (Flask):**
   - Represents the user interface or client side.
   - Built with Flask, a lightweight web framework for Python.
   - Responsible for rendering web pages and user interaction, including the form for querying the backend.

2. **Backend (FastAPI):**
   - Represents the server or backend of the application.
   - Built with FastAPI, a modern web framework for building APIs with Python.
   - Handles requests from the frontend, including querying birthdays and providing the current date.

3. **Docker Compose:**
   - Orchestrates the deployment of both frontend and backend as separate containers.
   - Ensures seamless communication between frontend and backend containers.
   - Simplifies the deployment and management of the entire application.

### Communication
Bidirectional communication is established between the Frontend (Flask) and Backend (FastAPI). Docker Compose facilitates this communication, allowing the components to work together seamlessly.

## Project Structure

- `backend/`: FastAPI backend implementation.
    - Dockerfile: Dockerfile for building the backend image.
    - main.py: Main backend application file.
    - requirements.txt: List of Python dependencies for the backend.
    - tests: Folder for testing code.
- `frontend/`: Flask frontend implementation.
    - Dockerfile: Dockerfile for building the frontend image.
    - static/: Folder for static files (CSS, JavaScript, etc.).
    - templates/: Folder for HTML templates.
    - main.py: Main frontend application file.
    - requirements.txt: List of Python dependencies for the frontend.
- `docker-compose.yml`: Docker Compose configuration for running both frontend and backend.

## Prerequisites
- Docker
- Visual Studio Code (Optional, for debugging)

## Usage
1. Clone the repository and navigate in the directory:

    ```bash
    git clone git@github.com:martina28mb/mcm_groupwork.git
    cd mcm_groupwork
    ```

2. Build and run the Docker containers:

    ```bash
    docker-compose up --build
    ```

    This will start both the frontend and backend containers.

3. Open your web browser and navigate to [http://localhost:8080](http://localhost:8080) to access the `frontend` and [http://localhost:8081](http://localhost:8081) to access the `backend`.

4. Click on the blocks in the home page to read informations about Veneto provinces and use the search bar to look for a city in Veneto region, in Italy. Suggested museums, if any, will be displayed below accomodations available in the city choosen.