
# A Simple Microservice using Go

## Overview
This project is a demonstartion of a simple microservice using golang.

## Features
This project involves generating a JWT token and validating it across two microservices running on different ports. The first service generates the token, while the second service validates it and displays a confirmation message upon successful validation, demonstrating secure inter-service communication.

## Dependencies
1.fmt: For printing formatted output.\
2.log: For logging information and errors.\
3.net/http: For handling HTTP server and client requests.\
4.os: For interacting with the operating system, such as reading environment variables.\
5.github.com/dgrijalva/jwt-go: For creating and parsing JSON Web Tokens (JWT)..



## Deployment

To deploy this project run

```bash
  git clone https://github.com/Srivastava-samarth/A-simple-microservice-using-go
```

Navigate to the Project Directory

```bash
  cd GO-SimpleMicroservice
```

Install the dependencies

```bash
  go mod tidy
```




## Documentation

In order to use this project there are couple of steps \
1.Navigate to the **`jwt-creator`** directory.\
2.Run the **`main.go`** file.\
3.Change directory to **`api`**.\
4.Run the **`main.go`** file.\
5.Generate a token by executing:
```bash
  curl localhost:8080
```
6.Copy the generated token.\
7.Validate the token by executing:
```bash
  curl -H "Authorization: Bearer <token>" localhost:9001
```



