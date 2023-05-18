# Read Me

## Description

A simple flask API connected to a React.js front-end. Based on: <https://www.youtube.com/watch?v=7LNl2JlZKHA&t=12s>

## Tutorial Notes

- use `npx create-react-app client` to stand up react app in a client folder
- create a folder for the flask server, and a `server.py` file for the server-side code.
- create a virtual environment (I used pipenv instead of venv) for the flask server
- Install the flask package as a dependency in the virtual env. (`pipenv install flask`)
- coded the backend.
- coded frontend.
  - removed the following files:
    - `index.css`
    - `app.test.js`
    - removed `logo.svg`
    - removed imports in `index.js` and `App.js`
- Updated `package.json` to include a `proxy` attribute (line 5). This should enable the react components to make relative path requests (i.e. without the domain name or localhost) instead of including that part for each request.
- Removed template code from `App.js` and replaced it with the react component template using VSCode's shortcut `rfce`.
- From the blank template, we created some state variables to hold the data from the API with `useState` hook.
-

## Take Aways

- Flask's standard output for JSON responses is in plain text. It doesn't have the same easy to read display as Django rest framework has it seems.
- The `proxy` connection seems to be either deprecated or may have changed, as, even though I followed the guide, it doesn't seem to retrieve data properly from the API.

## To Dos

- investigate how to set up `proxy` API endpoint for requests and fetching data.
