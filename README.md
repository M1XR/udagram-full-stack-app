Static Website click [here](http://udagram-ui-bucket-2022.s3-website-us-east-1.amazonaws.com)

URL: http://udagram-ui-bucket-2022.s3-website-us-east-1.amazonaws.com

# Hosting a Full-Stack Application

## Description

This is the final project from Udacity's FullStack JS Nanodegree. The goal is to deploy a 3-level full stack application on AWS and automate the deployment process with a CircleCI pipeline.

### Udagram

I have choosen to use the given Udagram-Starter-Project instead of using an own project.

## Usage

Udagram is a Insta-like Web-app where you can upload pictures. First you have to register an account. After you done this you can upload you favorite pics!

## Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

## Installation & Build

### install

- clone this repo
- navigate in your terminal to the root directory
- run
  - `npm run frontend:intall` to install frontend dependencies
  - `npm run api:install` to install backend dependencies

### build

- run in root
  - `npm run frontend:build` to build the frontend
  - `npm run api:build` to build the backend

## Start app on local

- In a first terminal navigate to `udagram/udagram-api` and run `npm start`.
- In a second terminal navigate to `udagram/udagram-frontend` and run `npm start`

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd udagram/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

## Deployment

### manually

- frontend: in root run `npm run frontend:deploy`
- backend: in root run `npm run api:deploy`

### automated

Push new commits to repo. This triggers the pipeline to start the deployment process.

### Unit Tests

Unit tests are using the Jasmine Framework.

### End to End Tests

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
