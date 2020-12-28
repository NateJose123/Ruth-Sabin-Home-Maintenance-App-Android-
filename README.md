# Ruth Sabin Home Maintenance App - Client Side

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
This project is an app that will enable residents of the Ruth Sabin Home to report maintenance issues so that the Darrin and Ray will be notified and know what needs to be addressed.

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Productivity
- **Story:** This app allows users to enter in details about maintenance issue, take a photo of the issue and report it.
- **Market:** This app targets the residents of the Ruth Sabin Home.
- **Scope:** The scope of This app will be having a robust login system to manage user info in case Darrin/Ray needs to contact them, a menu with fields for the user to fill in and submit details about the issue and an account management page so that the user's contact info is up to date.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**
* [ ] User must be able to register a new account
* [ ] User must be able to sign in
* [ ] User must be able to take a photo of issue
* [ ] User must be submit maintenance issue information
* [ ] Account Settings page UI must be completed
* [ ] Finish the settings backend (user able to change their username in settings)

**Optional Nice-to-have Stories**
* Stats about user issues reported.
* Notification when issue has been resolved.


### 2. Screen Archetypes

* Login Page
   * User must be able to sign in
   * User must be able to automaticlly be logged in
* Register
   * User must be able to register a new account
* Reporting Page
   * User can enter in maintenance info
   * User can take a picture of problem
* Settings
   * User can manage/update account and contact information.

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Reporting Page
* Account Settings

**Flow Navigation** (Screen to Screen)

* Login Page -> Account creation if no login is available
* Reporting Page -> Enter in maintenance info, take photo and submit.
* Account Settings Page -> Toggle Settings
 
## Wireframes
<img src="https://imgur.com/DKSrxn0.jpg" width="300" height="300">

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 
### Models
User
| Property       | Type.        | Description  |
| :------------- | :----------: | :----------- |
|  objectID      | String       | unique id for the user    |
|  UserName      | String       | what the user uses to login    |
|  Password      | String       | the user's login password |
|  ProfilePic    | File         | image for the user |
|  Email         | String.      | to help verify the user and send them emails |
|  Phone         | String.      | for Darrin/Ray to contact them if necessary |

Issues
| Property       | Type.        | Description  |
| :------------- | :----------: | :----------- |
|  objectID      | String       | unique id for the issue    |
|  IssueTitle    | String       | title of issue    |
|  IssueDesc     | String       | description of issue |
|  IssueSeverity | String       | severity level of issue |
|  IssuePic      | File         | picture of issue |
|  IssueLoc      | String       | location of issue |

