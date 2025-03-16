# ServerestAPI Automation test suite - Newman
## Overview
This project consists of an automation test suite designed to test APIs using Newman, a command-line tool for Postman. The tests are executed in a CI/CD pipeline to ensure that the API endpoints function as expected. The tests have been uploaded to GitHub for easy access and integration.

## Features
- API Test Automation: Automate API tests using Postman collections and execute them through Newman.
- Command-Line Execution: Execute tests directly from the command line or CI/CD pipeline.
- Customizable Reports: Generate detailed HTML of test execution reports.
- CI/CD Integration: Easily integrate the test suite into a CI/CD pipeline to automate testing with each code deployment.

## Documentation
- API: [Swagger](https://serverest.dev/#/)
  
## Prerequisites
Before running the tests, ensure that you have the following:
- Node.js: Newman requires Node.js. You can download it from [Node.js official website](https://nodejs.org/);
- Newman: Install Newman globally via npm:
`npm install -g newman`
- Postman Collection: The Postman collection file (.json) that contains the API tests should be available in the project repository.

## Running locally on Postman
### On Postman web or desktop
- Import a collection and the environment;
- Select them on Postman;
- Run the Collection. 

## Running Tests on Newman
To execute the test:
- Open the Terminal and go to your project folder
- Run the comand line:
`newman run Serverest.dev.postman_collection.json -e ServeRest.postman_environment.json -r cli,htmlextra`
This command will run the test suit and generate a html file that can be opened on any browser.

##License
This project is licensed under the MIT License.
