
Group Project - README Template
===

# Expecting

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description

To remind pregnant women to do the various things they need to do to have a healthy pregnancy.

### App Evaluation

- **Category: Health and Lifestyle**
- **Mobile:**
- **Story:**
- **Market: Pregnant Women**
- **Habit:**
- **Scope:**

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User can register and login (done)
* User can add name, age, weeks pregnant
* User can add information given from doctor

**Optional Nice-to-have Stories**

* Ring alarm when time to eat or take required medication
* Reminder of when you should go to bed
* Encouraging reminders sent throughout the day


### 2. Screen Archetypes

* The Login or Register
   * User can login
   * Creates username and password
   
* User Data Input
   [X] User adds age, weeks pregnant
   [] User can add if they are on multivitamins
   [] User can add a bedtime
   [] User can enter if they are physically
   [] User can add what time they would like to be reminded of all these things

* Home Page
   
### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home
* Schedule
* Edit Profile

**Flow Navigation** (Screen to Screen)

* Login
   * Takes User to home page if already signed up
   * If sign up button is tapped the user will be taken to the registration page
       *Username and password creation page
       *Personal Info
       *Maternal Welfare page
       *Then to Homepage
* Home Page
   * From home page the user navigate to the schedule page
   * From home page the user navigate to the edit profile page
   * From home page the user can logout

## Wireframes

<img src="https://i.imgur.com/41dXEGu.jpg" width=600 >

### [BONUS] Digital Wireframes & Mockups!
<img src="https://i.imgur.com/sB6dYim.jpg" width=600 >

### [BONUS] Interactive Prototype

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='http://g.recordit.co/OoCElfrSOo.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

## Schema 
[This section will be completed in Unit 9]
### Models
**Posts**
| Property | types | Description |
| --- | --- | --- |
| Reminder | String | Unique notification to the user |
| Profile | String | User information |
| Additional Notes | String | Additional details information for reminder |
| Time | Date and Time | User will get remind at a specific time |
| Reminder Name | String | Title of Reminder |
| URL | Hyperlink | Add links |
| Image | File | Image user attach |
### Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]

```
let query = PFQuery(className: "Items")
        query.includeKeys(["title", "dateTime", "description", "status"])
        query.limit = 20
        query.findObjectsInBackground { (posts, error) in
            if items != nil {
                self.items = items!
                self.tableView.reloadData()
            }
        }
```


    
- [OPTIONAL: List endpoints if using existing API such as Yelp]
