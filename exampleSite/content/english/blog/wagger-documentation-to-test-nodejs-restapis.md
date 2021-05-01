+++
author = "M D PUNEETH REDDY"
bg_image = "/images/node_cover-1.jpg"
categories = ["nodejs"]
date = 2021-04-03T18:30:00Z
description = "Swagger documentation for Nodejs RestAPIs, along with setups and example for both json and yaml formats with detail explanation."
draft = true
image = "/images/node_cover-1.jpg"
tags = ["expressjs", "nodejs", "swagger", "typescript"]
title = "WAGGER DOCUMENTATION TO TEST NODEJS RESTAPIS"
type = "post"

+++
We need to test our APIs without frontend, In this blog, we are going to see how to test Restful APIs with swagger.

## PREREQUISITES:

1. Nodejs express initial setup

If you want to know how to setup Nodejs RestAPI with expressjs you can see [here](https://mdpuneethreddy.com/expressjs-how-to-start-with-nodejs-and-expressjs/)

There are so many different ways to test APIs:

1. Swagger
2. postman

We can test with the [postman](https://www.postman.com/), it is a very good tool to test the APIs without a frontend, the other hand swagger helps us to document and test by creating an interface for the APIs and also we can test with that, its an important asset in the company’s to document the APIs and also to test the API along with it.

## **HOW CAN WE ADD SWAGGER DOCUMENTATION TO THE APIS**

we can document swagger in 2 different ways,

1. [JSON](https://en.wikipedia.org/wiki/JSON)
2. [YAML](https://en.wikipedia.org/wiki/YAML)

we can use any one format to add documentation for the APIs, Here we will discuss both the format of writing documentation, first, we will set up the swagger and give examples for both styles.

you can get complete code from my [Github](https://github.com/MDPuneethReddy/swagger_node), you can check it out here.

**Swagger documentation with JSON format:**

## **STEP1: INSTALL THE DEPENDENCIES**

first, we need to add the packages required to generate the swagger documentation they are swagger, swagger-doc, swagger-ui-express

Yarn add swagger swagger-jsdoc swagger-ui-express

After installing the dependencies you can see in the package.json like this in the dependencies

![swagger js doc packages](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image.png =418x90)

if you are using typescript for the backend Nodejs RestAPI, you need to install types for your project, the types for swagger-jsdoc and swagger-ui-express

Yarn add @types/swagger-jsdoc @types/swagger-ui-express

![](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-1.png =466x60)

## **STEP 2: ADD CONFIGURATION TO JSON FILE**

We need to configure the documentation how it should look, we will go set by step

![swagger config setup](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-2.png =751x572)

1. here the first open API is the swagger documentation version, you can check the official documentation for that
2. Next is the info about the API that needs to have about the API, here the swagger is more about the documentation of the API, so we need to make sure that none missing in the documentation to look into code,
3. In the components section we add the security schemas here we can add security to the documentation, in company's it is a must, there are different types of securities given to the swagger you can choose based on the use case

Next, we can also add the servers that need to set up and respond, we can add as many responses as we need, below you can see the URL, you can add as many URLs as you need

![servers add to swagger setup](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-3.png =594x401)

## **STEP 3: SETUP THE DEPENDENCIES**

1. import the JSON file into the main root file
2. next set up the document to swagger
3. Here you can see below the line where the path “/api” refers we can see the documentation at that URL, you can give your own path as you want.

![swagger import to main file](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-5.png =820x284)

So when you run the application and check the path, you can see like the below image, here you can add routes and schemas as you want

![image after running swagger](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-7-1024x306.png =1024x306)

## **SWAGGER DOCUMENTATION WITH YAML FORMAT:**

The difference between the JSON and Yaml format is the file format and another package to support Yaml format,

The basic setup is the same we will convert the same JSON file into a YAML file and configure it with the setup

## **STEP 1: MAKE A YAML FILE FOR THE CONFIGURATION**

We rewrite the config file above in JSON file to YAML file so you can get a good understanding of this,

![yaml file config ](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-11.png =621x448)

## **STEP 2: INSTALL YAMLJS :**

we need to install yamljs package to help to integrate the YAML file with the swagger setup

Yarn add yamljs

if you are using typescript you need to add the scripts for yamljs

**yarn add @types/yamljs**

## **STEP 3: ADD THE SETUP TO MAIN ROOT FILE**

![yaml setup swagger doc](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-9.png =803x356)

I just commented out the JSON file to show the difference, here the difference is to load the YAML file we need to use yamljs package and that's it the rest is the same and after this when you run the application you can see the same output as of JSON.

## CONCLUSION:

Here we have discussed how to install and set up the dependencies for the swagger documentation along with both formats with JSON and YAML for both typescript and javascript.

If you have any comments please write in the comments or reach out to me through contact or any suggestions to improve and anything wrong please write in comments. If you like this content, please share it with others

If you want to know how to setup Nodejs RestAPI with expressjs you can see [here](https://mdpuneethreddy.com/expressjs-how-to-start-with-nodejs-and-expressjs/)