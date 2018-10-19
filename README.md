# octopus

This project aims to build a tool able to run various type of tests and link them together to be able to investigate in case of test failure where is the test failing.

#Test all

## Client side

Octopus must be able to run selenium or similar UI test tool for integration tool but also have access to source code in order to run unit tests

## MDW side

Octopus must be able to run server side API test using REST, GraphQL, SOAPXML, RPC or any other API style. It must also have access to the source to run the unit tests

# Side feature

### Proxy

Octopus comes with a proxy that must be injected in the server and the UI. This server will allow 2 things
* Monitor the calls to the server from the UI or from the server to another server.
* Mock the response when investigation mode is turned on

### Database

Octopus comes with a data layer allowing
* Data injection before tests
* Modification of the behavior of the server in case of investigation

### Logs
Octopus will expose a log entrypoint
* To inject log when starting the tests to monitor what is happening during a test
* Check errors inside the logs to investigate (detect a class and run the unit test on it)

# Objectives

* Run and monitor the quality of a Single Page Application
* Investigate quickly what is happening
* Raise clear issue to developers to have a quick fix
* Improve test by detecting lack of coverage

# Status

This is currently only an idea. please contact me krysalead[at]gmail.com
