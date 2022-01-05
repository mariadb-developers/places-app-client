
This repository contains the a simple web application front-end application, built with React.js, called `Places`. The `Places` front-end communicates with a back-end API project (which should already be up and running when this app is started).

## Build and run the app

To start and run this application you need to execute the following commands within the root folder of this repo.

1. Install the Node.js packages (dependendies) for the app.

    ```bash
    $ npm install
    ```

2. Add your [Google API Key](https://developers.google.com/maps/documentation/javascript/get-api-key) to a new [environmental](https://www.npmjs.com/package/dotenv) (called `.env`) file to the root of this project.

      ```
      $ touch .env
      ```

      Then add the key `REACT_APP_GOOGLE_API_KEY`.

      ```
      REACT_APP_GOOGLE_API_KEY=<google_api_key_here>
      ```

      **Note:** The `REACT_APP_GOOGLE_API_KEY` environmental variable is used [here](src/components/MapContainer.js#L250).

3. Run the the app, which will available via http://localhost:3000.

    ```bash 
    $ npm start
    ``` 

## API Projects

This repo is configured as a [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) within the following repos:

* [places-app-nodejs](http://github.com/mariadb-developers/places-app-nodejs)
* [places-app-python](http://github.com/mariadb-developers/places-app-python)
* [places-app-jdbc-spring](http://github.com/mariadb-developers/places-app-jdbc-spring)
* [places-app-r2dbc-spring](http://github.com/mariadb-developers/places-app-r2dbc-spring)




