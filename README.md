# TestNodeServer
This is a test node REST server 

The example API has just two endpoints/routes to demonstrate authenticating and accessing a restricted route with basic authentication:

    /users/authenticate - public route that accepts HTTP POST requests containing the username and password in the body. If the username and password are correct then the user details are returned.
    /users - secure route that accepts HTTP GET requests and returns a list of all the users in the application if the HTTP Authorization header contains valid basic authentication credentials. If there are no basic auth credentials or the credentials are invalid then a 401 Unauthorized response is returned.
