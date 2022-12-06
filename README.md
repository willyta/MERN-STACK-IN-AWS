# MERN-STACK-IN-AWS
### This project shows the implementation of a web solution based on the MERN stack(ToDo App) in AWS Cloud. This project makes use of MongoDB DaaS

## STEP 0 - Prerequisite
In order to complete this project, you will need an AWS account and a virtual server with Ubuntu Server OS.

## STEP 1 – BACKEND CONFIGURATION
Update a list of packages in package manager

```
sudo apt update 
```

Upgrade ubuntu

```
sudo apt upgrade 
```

Get the location of Node.js software from Ubuntu repositories.

```
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - 
```

Install Node.js with the command below

```
sudo apt-get install -y nodejs
```

*Note: The command above installs both nodejs and npm. NPM is a package manager for Node*

Verify the node installation

```
node -v
```
```
npm -v
```
Create a new directory for your To-Do project and move into the directory
```
mkdir Todo && cd Todo
```
Clone the repository 

``` 
git clone https://github.com/willyta/MERN-STACK-IN-AWS.git
```
Initialise your project
```
npm init
```

Install ExpressJs and dotenv

```
npm install express dotenv

```
*we need to open port 5000 in EC2 Security Groups*

##MONGODB DATABASE

Create a file in your Todo directory and name it .env.
`touch .env`
`vi .env`

Add the connection string to access the database in it, just as below

`DB = 'mongodb+srv://<username>:<password>@<network-address>/<dbname>?retryWrites=true&w=majority'`

*NOTE Allow access to the MongoDB database from anywhere (Not secure, but it is ideal for testing) and make sure you change the time of deleting the entry from 6 Hours to 1 Week*

## STEP 2 – FRONTEND CREATION

In the same root directory as your backend code, which is the Todo directory, run:
```
npx create-react-app client
```
Install nodemon and concurrently

```
npm install concurrently nodemon --save-dev
```

Install Axios
```npm install axios```

Go to the Todo directory
`cd ../..`

When you are in the Todo directory run:

```
npm run dev
```








