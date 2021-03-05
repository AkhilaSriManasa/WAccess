# WAccess

## What is WAccess?
1. WAccess is a Google Chrome plug-in, that evaluates accessibility of websites based on some of WCAG 2.1 and WCAG 2.0 Guidelines.
2. The current version validates website based on 9 WCAG 2.1 and 8 WCAG 2.0 Guidelines.
3. Other WCAG 2.1 guidelines could also be included in the future versions.

## Features of WAccess:
1. Classifies all the 8 WCAG 2.0 and 9 WCAG 2.1 guidelines into four categories.
2. Displays list of violations on the console.
3. Also, displays relevant suggestions to fix the violation.

## Uses of WAccess:
There is massive digitization in the present day, leading to numerous websites.

Accessibility is one of the important features of these websites.

The WCAG guidelines could support the development of accessible websites.

Evaluating the websites against the WCAG guidelines could help in identifying violations against the WCAG guidelines, and could consequently help developers in developing accessible websites.

## Working of WAccess:
WAccess has been developed in Javascript, following the approach below:  

<img width="507" alt="wAc (1)" src="https://user-images.githubusercontent.com/42757231/110108104-c6b01f00-7dd1-11eb-9695-c12cd3255aa5.PNG">

WAccess considers 9 WCAG 2.1 guidelines and 8 WCAG 2.0 guidelines, which do not require human intervention, as shown in the following Table, to evaluate the accessibility of a website. 

We integrate these guidelines into 4 classes - (i) aria-related, (ii) color-contrast related, (iii) HTML-check related and (iv) interaction-related.

These guidelines are reviewed to identify and sort the best practices required to meet the criteria of all guidelines. 

Based on the best practices observed, rules are defined to evaluate a webpage against the specified criteria. 

Scripts to check the accessibility of a website based on the rules defined is written using JQuery. 

Each of these scripts are designed to address one accessibility guideline. 

All the scripts are then compressed and bundled together into a single .js file named as background.js. 

A manifest.json file is built to run the background.js file. 

All these files are bundled together as the WAccess plugin.


## WCAG Guidelines considered:

<img width="352" alt="tabWacc" src="https://user-images.githubusercontent.com/42757231/110108814-a5036780-7dd2-11eb-8730-cb18311fef6b.PNG">


## What's inside WAccess Repository:
In the "accessibility-chrome-plugin" folder,   

"js" folder contains list of all ".js" files.

"background.js" file contains all the bundled source code related to preprocessing website, evaluating the website and generating suggestions for the violated guidelines.

"accessibility-build.js" file contains the source code required to display violated guidelines and corresponding suggestions on the console.

"screenshots" folder includes the screenshots of evaluation of a government website - UIDAI (uidai.gov.in).

"manifest.json" file includes the url that triggers start of WAccess and other application related data.


## Steps to install WAccess:
1. Download the repository on your local machine.  
2. Unzip the folder and extract it to a location of your choice on your PC.  
3. Now, open Google Chrome and Go to Settings  
4. Select Extensions or navigate to chrome://extensions  
5. Turn on Developer Mode at the right side top corner of chrome://extensions  
6. Click on “Load unpacked”  
7. A popup appears to select folder  
8. Select WAccess folder from the location you previously extracted to, and click on OK.  
9. WAccess Plugin gets installed on Chrome.  

## Steps to use WAccess:
1. Navigate to any website of your choice 
2. Right Click and select 'Accesibility Test' on any website
3. Check Errors and Warnings in the Console


## How to contribute to WAccess
We will be very happy to receive any kind of contributions. Incase of a bug or an enhancement idea or a feature improvement idea, please open an issue or a pull request. Incase of any queries or if you would like to give any suggestions, please feel free to contact Akhila Sri Manasa Venigalla (cs19d504@iittp.ac.in) or Sridhar Chimalakonda (ch@iittp.ac.in) of RISHA Lab, IIT Tirupati, India.
