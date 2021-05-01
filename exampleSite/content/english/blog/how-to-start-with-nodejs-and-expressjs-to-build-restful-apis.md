+++
author = "M D PUNEETH REDDY"
bg_image = "/images/node_cover.jpg"
categories = ["Nodejs"]
date = 2021-03-31T18:30:00Z
description = "Expressjs and nodejs backend API beginner start to create small API and run locally to test the frontend applications."
draft = true
image = "/images/node_cover.jpg"
tags = ["typescript", "expressjs", "Nodejs"]
title = "HOW TO START WITH NODEJS AND EXPRESSJS TO BUILD RESTFUL APIS"
type = "post"

+++
Get started with Nodejs backend with Expressjs, In this blog, we are going to learn about how to start the backend server or rest API locally. It's just a beginner blog post where we just start our server. Before reading this block check out the prerequisites below to install Node and yarn or npm package manager, after Installing them start with the blog.

## PREREQUISITES:

* Install [NODE](https://nodejs.org/en/download/)
* Install [YARN](https://yarnpkg.com/getting-started/install) or [NPM](https://www.npmjs.com/get-npm)

follow the steps,

## SETUP:

## **STEP-1:**

Now start creating a blank repository in your system and go to that repository

mkdir foldername

Cd foldername

## **STEP-2:**

We need to create a backend initial template in this blog I will show you with Yarn,

Enter “Yarn init” and enter, it will ask the template questions, you can just click enter for all the questions, the default template will be created

Yarn init

![expressjs template](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-12.png =377x173)

then you can see the below file will be created in the directory, it is the package.json file where we can see all the packages installed information

![package.json file in folder](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-13.png =602x71)

## **STEP-4**:

For starting the server you need to install expressjs, expressjs is a framework used for nodejs backend server

Yarn add expressjs

After installing expressjs, open your favorite code editor and open the folder, When you open the folder you can see it like this.

![nodejs folder structure](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-15.png =239x256)

Now we can write your code to create the server, Now I don’t have any file to write the code, we need to create a file, The easy method is to go to package.json and check the main

![check initial file](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-16.png =298x241)

Here I have the file name as index.js, the initial point to the server to run the code is index.js, There are two options.

1. Here you can give your own file name and create a file in the repository

2\. Just create the name based on the name that corresponds to the main in package.json

If we go with the different name change “index.js” the file name beside main to your own Filename “yourname.js” and create a file in the repository.

![expressjs own initial file](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-17.png =602x244)

## **STEP-5:**

For the blog we will go with “index.js”, create a file index.js in your repository

![expressjs default initial file](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-18.png =602x221)

## SERVER CODE WITH EXPRESSJS

## **STEP-6:**

Just we need a couple of lines of code to start your server, First “import express “, next “const app=express() ” creates a new application for you, following make that app to list at port 3000 or any port

![expressjs API start code](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-19.png =602x148)

## **STEP-7:**

Run the command- “node index.js”, you can see the console

**node index.js**

After running the above command you can see the below image running at port 3000

![console look for running api](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-20.png =296x34)

That’s it your server is running at port 3000, go to the browser and enter [http://localhost:3000/](http://localhost:3000/), you can see like this,

![check get request in browser](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-21.png =356x99)

Here you can see your localhost is running but there is nothing to show a response from the server at localhost, so we add small code

## **STEP-8**:

Add app. get(“/”) method, here app. get() means whenever this app is called with getting method with the path “/”, here “/” indicates the initial path,

![add get request for the api](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-22.png =516x248)

## **STEP-9**:

Next stop the server and restart again node index.js, you can see “welcome to API”

![expressjs welcome to api](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-23.png =455x121)

Now our backend server is running, you could have observed that you restarted the app again after saving changes, so it is annoying to restart every time you made changes, so will set up some package which will take care of it I,e ”Nodemon”

## **STEP-10:**

Add package nodemon to the application

Yarn add nodemon

## **STEP-11:**

While it installing go to package.json add the “start script”

![nodemon script](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-24.png =363x382)

## **STEP 12:**

After installing nodemon, run yarn start in the command line, you can see nodemon running automatically, you can write code if any changes nodemon checks and restart again, ignore that warning for now

Yarn start

![expressjs nodemon start](https://mdpuneethreddy.com/wp-content/uploads/2021/04/image-26.png =602x195)

That’s it for the blog, if you have any questions write them down below

## **CONCLUSION:**

Here in this blog, we learned how to Start our own backend server locally using expressjs, nodejs. If you have any doubts or questions please write to me, you can comment down below. Any suggestions to Improve from my side you can write in comments too.

please check for technology blogs [here.](https://mdpuneethreddy.com/category/technology/)

If you liked the blog please share it with your friends.