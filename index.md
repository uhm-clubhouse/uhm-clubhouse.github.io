# UHM Clubhouse

## Table of contents

* [Overview](#overview)
* [Features](#features)
* [User Interface Mockups](#user-interface-mockups)
* [Deployment](#deployment)
* [Continuous Integration](#continuous-integration)
* [Development History](#development-history)
* [Team](#team)


## Overview 
Finding and learning about student clubs that are available at UH Manoa is a difficult task that the UHM Clubhouse intends to solve. The UHM Clubhouse is an application for students to browse an organized directory of all current student clubs with brief descriptions, meeting information, URL to their websites, contact information, and a few select photos.

## Features
* Three distinct user roles
  * Regular users can enjoy a seamless browsing experience of the directory
  * Club admins wield the power to edit their club's data
  * Super admins play the crucial role of ensuring site content appropriateness and bestowing "club admin" privileges upon chosen users
* Browsing page
  * Filter clubs based on interest areas, such as "athletic," "art," and "music." 
  * A club can belong to multiple interests areas
* Notifications
  * Users receive notifications based on their interest areas
    * New club that matches to their preferences
    * When an existing club adds an interest area relevant to the user
* Admin responsibilities
  * Review site content to ensure it is appropriate
  * Introduce new categories, such as musical tastes, capabilities, and goals


## User Interface 
This section provides a walkthrough of the UHM Clubhouse user interface and its capabilities.

#### Landing Page
The landing page is the very first page presented to all users who are not logged in. Users can learn about the UHM Clubhouse application and log in or sign up.

Planned design:
<img src="images/landing.png">

M1 update (11/16):
<img src="images/m1-landing1.png">
<img src="images/m1-landing2.png">


#### Profile Creation and Login Page
This is where users can input their first and last name, email, and password to create a new account. Existing users can also log in by clicking the "Login" button in the top right corner to input their email and password.

Planned design:
<img src="images/signin.png">

M1 update (11/16):
<img src="images/m1-signin.png">

#### User Home Page
This home page is presented to users who are logged in. Recent updates are shown in the center of the page, along a sidebar containing a searchbar and a list of the clubs the users are following. Users can also access the "Club Listing" and "Create Club" links in the navigation bar on the top of the page.

Planned design:
<img src="images/user-landing.png">

M1 update (11/16):
<img src="images/m1-userlanding.png">

M2 update (11/28):
<img src="images/m2-userlanding.png">

#### Club Listing Page
This page is the listing page, where users can browse all the available clubs that are posted. Specific clubs can be searched through the searchbar and club listings can be filtered to fit the user's needs. 

Planned design:
<img src="images/club-listing.png">

M1 update (11/16):
<img src="images/m1-userclublisting.png">

M2 update (11/28):
<img src="images/m2-clublisting.png">

#### Club Creation Page
This page is the club creation page, where users can create a posting for their club. 

Planned design:
<img src="images/create-club.png">

M1 update (11/16):
<img src="images/m1-createclubs.png">

M2 update (11/28):
<img src="images/m2-createclub.png">

Form is submittable:
<img src="images/m2-createclubform.png">


Upon submitting a form, data is written to the database:

ClubsCollection:
<img src="images/m2-write1.png">
ClubsInterestsCollection:
<img src="images/m2-write2.png">

#### Club Admin Home Page
Users with the Club Admin role can view all of their club postings and have the ability to edit the data associated with their club.

Planned design:
<img src="images/edit-club.png">

M1 update (11/16):
<img src="images/m1-useryourclubs.png">

M2 update (11/28):
<img src="images/m2-clubadmin.png">

Your Clubs tab:
<img src="images/m2-editclub.png">
<img src="images/m2-editclubform.png">

#### Super Admin Home Page
Users with the Super Admin role are responsible for making sure the site content is appropriate and are able to delete a club posting at any time. Additionally, they are able to grant "Club Admin" privileges to selected users via the link in the navigation bar.

Planned design:
<img src="images/super-admin.png">

M2 update (11/28):
<img src="images/m2-sadmin.png">
<img src="images/m2-sadminset.png">

## Deployment
We’ve deployed our application, which can be found [here](https://uhm-clubhouse.xyz/)
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
* Creating necessary documentations and presentations

### [Milestone 2](https://github.com/orgs/uhm-clubhouse/projects/5)
* Have pages load default data
* Edit the design of each page to match mockups
* Have the Create Club form write data to the database
* Deploy four pages in addition to the landing page

### [Milestone 3](https://github.com/orgs/uhm-clubhouse/projects/6)
* Improve functionality of the system
* 
     
## Team
UHM Clubhouse is designed, implemented, and maintained by [Miki Kojima](https://github.com/miki-x2), [Keiko Raiola](https://github.com/keikotr), [Iverson Yago](https://github.com/iversony1), [Lizyl Failano](https://github.com/lizylf), [Delsin Rhoney](https://github.com/DelsinRhoney), [Chad Vilayvong](https://github.com/Chadv2). 

These members have signed a contract for this organization, which can be viewed [here](https://docs.google.com/document/d/17iacQBDx85FvQOAC1Jws0_lws82LN-tlW3v9oX7Rp2A/edit?usp=sharing).


