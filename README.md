# Server less flask

A sample project built with flask and deployed via serverless framework to aws lambda.

After cloning this project follow these steps

## Install python dependencies

```shell
pip install -r requirements.txt
```

## Install node dependencies

```shell
npm i -g serverless
npm i
```

## AWS configure
```shell
aws configure 
#enter your IAM access key, secret, default region and out format to json
```

## Serveless deploy
```shell
serveless deploy
```

## Generate requirement txt
If you want some more dependencies install them and use following
The requirement.txt needs to be in UTF-8 or serverless deploy fails
```shell
#in powershell in windows
pip freeze | Out-File -Encoding UTF8 requirements.txt 
```

Reference: https://www.serverless.com/blog/flask-python-rest-api-serverless-lambda-dynamodb/
