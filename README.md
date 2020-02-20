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
* You can find the API ID and Resourse ID on top of the API Gateway screen
* The ID next to the API name is the API ID(q46soknj3c). 
* The ID right of the ‘Resource’ is the root resourceID(uuni865ulk).
