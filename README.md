# allureSamples
Generating Allure reports on multiple test frameworks in multiple languages
# flow
Flow repo for services

## API reference doc
https://docs.google.com/document/d/1s02BdysL3xrHD9U8knDW_6gvqPovD3AhsurlkYtdDhM/edit?usp=sharing

`GO Version: golang:1.13.4`

### TODO
- [x] One Click Deploy - Makefile with docker
- [x] Pass libs integration [use wiki]
- [x] Tenant service API  
- [x] Write Tests using mocks 
- [x] Constants declaration
- [ ] All services - Common Response Messages   
- [ ] Middleware - versioning of API's
- [ ] Mysql json field from GO model 
- [ ] sql to sqlx

### How To Run This Project
> Make Sure you have run the flow.sql in your mysql


Since the project already use Go Module, you can put the source code in any folder but GOPATH.

#### Run the Applications
Here is the steps to run it with `docker-compose`

```bash

#move to project
$ cd flow

# Build the docker image first
$ make docker

# Run the application. This will launch both mysql & flow services
$ make run 

# check if the containers are running
$ docker ps

# Execute the call
$ curl localhost:12001/tenant?name=paas

# Stop
$ make stop
```

#### Run the Testing

```bash
$ make test
```
