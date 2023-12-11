# UHM Clubhouse

## Table of contents

* [Overview](#overview)
* [Features](#features)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Deployment](#deployment)
* [Developer Guide](#developer-guide)
* [Continuous Integration](#continuous-integration)
* [Development History](#development-history)
* [Team](#team)


## Overview 
Finding and learning about student clubs that are available at UH Manoa is a difficult task that the UHM Clubhouse intends to solve. The UHM Clubhouse is an application for students to browse an organized directory of all current student clubs with brief descriptions, meeting information, and contact information.

## Features
* Three distinct user roles
  * Regular users can enjoy a seamless browsing experience of the directory
  * Club admins wield the power to edit their club's data
  * Super admins play the crucial role of ensuring site content appropriateness and bestowing "club admin" privileges upon chosen users
* Browsing page
  * Filter clubs based on interest areas, such as "athletic," "art," and "music." 
  * A club can belong to multiple interest areas
* Notifications
  * Users receive notifications based on their interest areas
    * New club that matches to their preferences
    * When an existing club adds an interest area relevant to the user
* Admin responsibilities
  * Review site content to ensure it is appropriate
  * Introduce new categories, such as musical tastes, capabilities, and goals


## User Guide
This section provides a walkthrough of the UHM Clubhouse user interface and its capabilities.

#### Landing Page
The landing page is the very first page presented to all users who are not logged in. Users can learn about the UHM Clubhouse application and log in or sign up.

![](images/m2-landing.png)


#### Profile Creation and Login Page
This is where users can input their first and last name, email, and password to create a new account. Existing users can also log in by clicking the "Login" button in the top right corner to input their email and password.

<img src="images/m1-signin.png">

#### User Home Page
This home page is presented to users who are logged in. Recent updates are shown in the center of the page, along a sidebar containing a search bar and a list of the clubs the users are following. Users can also access the "Club Listing" and "Create Club" links in the navigation bar on the top of the page.

![](images/m2-userlanding.png)

#### Club Listing Page
This page is the listing page, where users can browse all the available clubs that are posted. Clubs can be searched using the search bar and club listings can be filtered by interest.

![](images/final-clublisting.png)

Filter function:
![](images/final-filterfunction.png)

Search function: 
![](images/final-searchfunction.png)

#### Club Creation Page
This page is the club creation page, where users can create a posting for their club. 

![](images/m2-createclub.png)

![](images/m2-createclubform.png)


#### Club Admin Home Page
Users with the Club Admin role can view their club postings and edit the club information.

![](images/m3-yourclubs.png)
![](images/m3-editclubs.png)
![](images/m2-editclubssuccess.png)

Club admin users can also search for their club postings by the search bar or by interest.

Filter Function:
![](images/m3-yourclubseditedinterest.png)

Search Function:
![](images/m3-yourclubseditedsearch.png)

#### Super Admin Home Page
Users with the Super Admin role are responsible for ensuring the site content is appropriate and can delete a club posting at any time. Additionally, they can grant "Club Admin" privileges to selected users via the link in the navigation bar.

![](images/m2-sadmin.png)
![](images/m2-sadminset.png)

## Community Feedback
After deploying the application, the team asked for feedback from the UH community using a Google Form found [here](https://forms.gle/AQyRCnFNsQDmtRi17). Below are some feedback we received from the community:

## Deployment
We’ve deployed our application, which can be found [here](https://uhm-clubhouse.xyz/)

## Developer Guide

### Installation
1. Install [Meteor](https://www.meteor.com/install).

2. Download a copy of [UHM Clubhouse](https://github.com/uhm-clubhouse/uhm-clubhouse) 
3. After downloading, cd into the app directory and install the required libraries:

    ``
    $ cd app
    ``

    ``
    $ meteor npm install
    ``
4. Once the libraries are installed, run the system by invoking
    ``
    $ meteor npm run start
    ``
5. If all goes well, the application will appear at http://localhost:3000

## Continuous Integration

![ci-badge](https://github.com/uhm-clubhouse/uhm-clubhouse/workflows/ci-uhm-clubhouse/badge.svg)

UHM Clubhouse uses GitHub Actions to automatically run ESLint and TestCafe each time a commit is made to the default branch. You can see the results of all recent “workflows” at https://github.com/uhm-clubhouse/uhm-clubhouse/actions.

The workflow definition file is quite simple and is located at [github/workflows/ci.yml](https://github.com/uhm-clubhouse/uhm-clubhouse/blob/main/.github/workflows/ci.yml)

## Development History
### [Milestone 1](https://github.com/orgs/uhm-clubhouse/projects/2)
* Create mockups for the user interface
* Setting up project home page
* Create default data
* Creating necessary documentation and presentations

  #### Planned Designs:

    Landing:
    ![](images/landing.png)
    
    Sign-in and Login:
    ![](images/signin.png)
    
    User Home Page:
    ![](images/user-landing.png)

    Club Listing Page:
    ![](images/club-listing.png)
    
    Club Creation Page:
    ![](images/create-club.png)

    Club Admin Home Page:
    ![](images/edit-club.png)

    Super Admin Home Page:
    ![](images/super-admin.png)


  #### Updated user interface:

    Landing:
    ![](images/m1-landing1.png)
    ![](images/m1-landing2.png)
  
    Sign-in and Login:
    ![](images/m1-signin.png)
  
    User Home Page:
    ![](images/m1-userlanding.png)
  
    Club Listing Page:
    ![](images/m1-userclublisting.png)
  
    Club Creation Page:
    ![](images/m1-createclubs.png)
  
    Club Admin Home Page:
    ![](images/m1-useryourclubs.png)

### [Milestone 2](https://github.com/orgs/uhm-clubhouse/projects/5)
* Have pages load default data
* Edit the design of each page to match mockups
* Have the Create Club form write data to the database
* Deploy four pages in addition to the landing page
* Implement continuous integration
* Test all deployed pages using TestCafe

  #### Updated user interface:

  Landing:
  ![](images/m2-landing.png)

  User Home Page:
  ![](images/m2-userlanding.png)

  Club Listing Page:
  ![](images/m2-clublisting.png)

  Club Creation Page:
  ![](images/m2-createclub.png)
  The form is submittable:
  ![](images/m2-createclubform.png)
  Upon submitting a form, data is written to the database:

    ClubsCollection:
  ![](images/m2-write1.png)

  ClubsInterestsCollection:
  ![](images/m2-write2.png)

  Club Admin Home Page:
  ![](images/m2-clubadmin.png)

  Edit Clubs:
  ![](images/m2-editclub.png)
  ![](images/m2-editclubform.png)

  Super Admin Home Page:
  ![](images/m2-sadmin.png)
  Set Admin:
  ![](images/m2-sadminset.png)

### [Milestone 3](https://github.com/orgs/uhm-clubhouse/projects/6)
* Improve the functionality of the system
* Clean up the user interface
* Additional testing of the system

  #### Updated user interface:

    Landing Page:
  * Updated logo and user interface
  ![](images/m3-landingpage.png)

    User Home Page:
  * Shows users their joined clubs
  * Added a join and leave club function
  ![](images/m3-userhomepage.png)
  ![](images/m3-userhomepageedited.png)
 
    Admin Request Form
  * Allows users to request to become a club admin via email address
  ![](images/m3-adminrequestpage.png)
    The request form is submittable:
  ![](images/m3-adminrequestpagesuccess.png)

    Club Listing Page:
  * Added a filter and search function
  * Added a leave club function
  ![](images/m3-clublisting.png)
  ![](images/m3-clublistinginterest.png)
  ![](images/m3-clublistingsearch.png)

    Your Clubs Page for Admins:
  * Added a filter and search function
  * Added a delete club function
  ![](images/m3-yourclubs.png)

    Edit Club Page for Admins:
  ![](images/m3-editclubs.png)
    After editing club information, the form is submittable:
  ![](images/m3-editclubssuccess.png)
    Edited club information appears on the "Your Clubs" page with filter and search functions working with the edited club:
  ![](images/m3-yourclubsedited.png)
  ![](images/m3-yourclubseditedinterest.png)
  ![](images/m3-yourclubseditedsearch.png)
    Edited club information appears on the "Club Listing" page with filter and search functions working with the edited club:
  ![](images/m3-clublistingedited.png)
  ![](images/m3-clublistingeditedinterest.png)
  ![](images/m3-clublistingeditedsearch.png)

    Admin Requests Page for Super Admins only:
  * Shows what accounts are requesting to be admins
  * Added a hide function to hide any admin requests
  ![](images/m3-adminrequest.png)
     
## Team
UHM Clubhouse is designed, implemented, and maintained by [Miki Kojima](https://github.com/miki-x2), [Keiko Raiola](https://github.com/keikotr), [Iverson Yago](https://github.com/iversony1), [Lizyl Failano](https://github.com/lizylf), [Delsin Rhoney](https://github.com/DelsinRhoney), [Chad Vilayvong](https://github.com/Chadv2). 

These members have signed a contract for this organization, which can be viewed [here](https://docs.google.com/document/d/17iacQBDx85FvQOAC1Jws0_lws82LN-tlW3v9oX7Rp2A/edit?usp=sharing).


