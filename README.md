# Sequelize Passport Example

This is included in the student facting content for unit 14. It is located at `04-Important/Sequelize-Passport-Example`. The students are instructed to use this app as the starter for Project #2.

I've created this repo in order to provide some version control separate from the main full-stack ground curriculum and to allow for demonstration deployment.

## Deployment

This app is configured for using GitHub with Travis CI for version control and CI. The project is ready for deployment on Heroku. A JawsDB instance must be provisioned for the Heroku app.

Add a `SERVER_SECRET` to the Heroku config for the app. (See [Configuration and Config Vars](https://devcenter.heroku.com/articles/config-vars) to learn how.)

## Running Locally

- Update username, password, and database fields in `/config/config.json` for local MySQL server connection.
- Create a `.env` file in the root folder of the project. The file must include the following:
  ```
  SERVER_SECRET = <your_secret_for_session_signing>
  ```
- Run `npm run watch` to start development server using nodemon.
