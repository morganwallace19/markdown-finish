### Hugo on Netlify Tutorial

### Tutorial Objective

The objective of this tutorial is to use Netlify to host a Hugo website using Visual Studio Code and Github.

### Getting Started

To get started:

![Node Installation Page](<tutorial screengrabs/tutorial 20.png>)

Install node from this URL: https://nodejs.org/en/download

 ![Node version in terminal](<tutorial screengrabs/node js 1.png>)
 
 Check the version of node using the command:
 > node --version

 ![Node version in Visual Studio Code](<tutorial screengrabs/node js 2.png>)

Also check the node version in Visual Studio Code as well.


Next Install Hugo by using the program installer 'Scoop'.

![Command to install scoop](<tutorial screengrabs/hugo 1.png>)

Install Scoop by using the command:
> iwr -useb get.scoop.sh | iex

![Command to install Hugo](<tutorial screengrabs/hugo 2.png>)

Use Scoop to install hugo:
> scoop install hugo-extended

![Hugo version command](<tutorial screengrabs/hugo 3.png>)

Check the hugo version on machine and VS code:
> hugo version


### Step 1 - Using Github to create a repository of a Hugo template

Step 1 involves using a template on Hugo from github.

![Hugo template on Github](<tutorial screengrabs/tutorial 1.png>)

Use the template to create a repository from Github.

![Repository created](<tutorial screengrabs/tutorial 2.png>)

Create the repository.


### Step 2 - Cloning the repository

Step 2 involves cloning the created repository with the Hugo template.

![Repository URL to clone](<tutorial screengrabs/tutorial 21.png>)

Copy the repository URL to clone.

![Repository clone command](<tutorial screengrabs/tutorial 3.png>)

Enter the following command to clone the repository into a folder:
> git clone https://github.com/morganwallace19/Hugo-test-three.git


### Step 3 - Using Visual Studio Code terminal to get Netlify to host the Hugo site

Step 3 involves using Visual Studio code to deploy a hugo site using Netlify.


![Repository folder Structure](<tutorial screengrabs/tutorial 4.png>)

The folder structure in Visual Studio Code.

![Netlify.toml file](<tutorial screengrabs/tutorial 5.png>)

The netlify configuration file.

![Hugo command](<tutorial screengrabs/tutorial 7.png>)

Enter the following command to get started with hugo:
> hugo

![Created public folder](<tutorial screengrabs/tutorial 6.png>)

Public folder is created when hugo command is entered.

![Localhost Hugo site](<tutorial screengrabs/tutorial 8.png>)

Enter this command to view the hugo site on localhost:
> hugo server-D

![Hugo server setup](<tutorial screengrabs/tutorial 9.png>)

Enter this command to set up a localhost using netlify:
> netlify dev

Then click on the dev command option that says:
> [Hugo] 'hugo server -w'

![Local server setup](<tutorial screengrabs/tutorial 10.png>)

This shows that process while the localhost server is being setup.

![Localhost setup](<tutorial screengrabs/tutorial 11.png>)

Once the setup is finished, you can now view the site on localhost:8888.

![Hugo localhost in browser](<tutorial screengrabs/tutorial 12.png>)

View the localhost on the browser.

![Index page](<tutorial screengrabs/tutorial 13.png>)

Before deployment, go to the index.html page in the public folder and make a couple of changes.

![Netlify deploy](<tutorial screengrabs/tutorial 14.png>)

Enter this commmand to begin site deployment:
> netlify deploy

Next select the options below:
? What would you like to do? + Create & configure a new site
? Team: (Name of team on Netlify dashboard)
? Site name: (enter what you would like your site to be named)

Site deployment begins.

![Deployed site in browser](<tutorial screengrabs/tutorial 15.png>)

View the deployed site in browser. Notice the HTTPS as well.

![URL clean](<tutorial screengrabs/tutorial 17.png>)

Enter this command to tidy the URL:
> netlify deploy --prod

![URL before](<tutorial screengrabs/tutorial 16.png>)
![URL after](<tutorial screengrabs/tutorial 18.png>)

Comparison between the two URLs. Before shows the URL but untidy and after shows the tidy URL with site name.

![Netlify dashboard](<tutorial screengrabs/tutorial 19.png>)

Go to your netlify dashboard and you should see the deployed site.


### End of Tutorial