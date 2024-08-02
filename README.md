# Note Taker Starter Code

## Description

This Note Taker application allows users to write, save, and delete notes. It's a simple and efficient way to keep track of tasks and organize thoughts. The application uses an Express.js backend to handle the storage and retrieval of notes from a JSON file.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Routes](#routes)
- [Screenshots](#screenshots)
- [Deployment](#deployment)
- [License](#license)

## Installation

1. Clone the repository:
    ```bash
    git clone <your-new-repository-url>
    cd <your-repository-name>
    ```

2. Install the necessary dependencies:
    ```bash
    npm install
    ```

3. Start the server:
    ```bash
    node server.js
    ```

## Usage

1. Open your browser and navigate to `http://localhost:3001`.
2. Click on the "Get Started" button on the landing page to navigate to the notes page.
3. On the notes page, you can:
   - View existing notes in the left-hand column.
   - Enter a new note title and text in the right-hand column.
   - Click the "Save Note" button to save a new note.
   - Click on an existing note to view it in the right-hand column.
   - Click the "New Note" button to create a new note.
   - Click the "Clear Form" button to clear the form fields.

## Routes

### HTML Routes

- `GET /notes` - Returns the `notes.html` file.
- `GET *` - Returns the `index.html` file.

### API Routes

- `GET /api/notes` - Reads the `db.json` file and returns all saved notes as JSON.
- `POST /api/notes` - Receives a new note to save on the request body, adds it to the `db.json` file, and returns the new note to the client.

## Screenshots

## Deployment

This application is deployed on Render. To deploy your own version, follow these steps:

1. Go to your Render dashboard.
2. Click on "New" and select "Web Service".
3. Connect your GitHub repository with the note-taking app.
4. Set the build command to `npm install`.
5. Set the start command to `node server.js`.
6. Click "Deploy".

