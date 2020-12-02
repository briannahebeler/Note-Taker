# Note-Taker

## Description

A notes application deployed on Heroku. This application allows the user to write, save, and delete notes so that they can organize their thoughts and keep track of tasks to be completed. This application will use an express backend and save and retrieve note data from a JSON file.

## Table of Contents  
* [Screenshots](#screenshots)
* [Contributing](#contributing)
* [Questions](#questions)
* [Links](#links) 

## Screenshots
![](./assets/screenshots/screenshot.png)

## Contributing
To contribute to this project you can fork this GitHub repository.

## Questions
If you have any additional questions about this application you can reach out to me at briannahebeler@gmail.com.
You can check out some of my other projects at briannahebeler (https://github.com/briannahebeler).

## Links

* Deployed Application: (This should be the link to the url provided by Heroku)

* GitHub Repo: https://github.com/briannahebeler/Note-Taker

## Directions

* The application frontend has already been created, it's your job to build the backend and connect the two.

* The following HTML routes should be created:

  * GET `/notes` - Should return the `notes.html` file.

  * GET `*` - Should return the `index.html` file

* The application should have a `db.json` file on the backend that will be used to store and retrieve notes using the `fs` module.

* The following API routes should be created:

  * GET `/api/notes` - Should read the `db.json` file and return all saved notes as JSON.

  * POST `/api/notes` - Should receive a new note to save on the request body, add it to the `db.json` file, and then return the new note to the client.

  * DELETE `/api/notes/:id` - Should receive a query parameter containing the id of a note to delete. This means you'll need to find a way to give each note a unique `id` when it's saved. In order to delete a note, you'll need to read all notes from the `db.json` file, remove the note with the given `id` property, and then rewrite the notes to the `db.json` file.