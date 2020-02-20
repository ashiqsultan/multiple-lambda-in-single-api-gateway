# multiple-lambda-in-single-api-gateway
This repo contains serverless.yml which you can copy and use to deploy multiple lambda functions in a single AWS API gateway


```
provider:
  apiGateway: # Optional API Gateway global config
    restApiId: q46soknj3c # This should be same for the other api being deployed to the same API Gateway
    restApiRootResourceId: uuni865ulk # This should be same for the other api being deployed to the same API Gateway
```
`restApiId` and `restApiRootResourceId` is the important thing to note

## Instructions
* Create new API Gateway in AWS console.
* Note down API ID and Resourse ID
* The ID next to the API name is the API ID(jte3ap5vzd). 
* The ID right of the ‘Resource’ is the root resourceID(63l279u23l).
