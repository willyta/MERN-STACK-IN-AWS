# MERN-STACK-IN-AWS
### This project shows the implementation of a web solution based on the MERN stack(ToDo App) in AWS Cloud.

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

Initialise your project
```
npm init
```

Install ExpressJs and dotenv

```
npm install express dotenv

```

tou





