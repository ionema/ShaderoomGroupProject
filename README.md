# NewsRoom

## TABLE OF CONTENTS 
1. [Overview](##Overview) 
2. [Product Spec](##ProductSpec)
3. [Wireframes](##Wireframes)
4. [Schema](##Schema)

## Overview

**Description**

A social media forum website that discusses news, gossip, and lifestyle for men and women ages 18 - 35.


**App Evaluation**
- **Category:** Social Networking / Music
- **Story:** Delivers news, gossip, and lifestyle posts to users. Gives users the ability to participate in group chats / forums  that discuss a given topic.
- **Market:** Men and Women ages 18 - 35
- **Habit:** This app should be used daily or as often as the user would like depending on how often the usr would like to research and discuss the news.
- **Scope:** First we would like to start by delivering the news and giving users a platform to discuss the news. Eventually we would like to provide our own news media and contents rather than getting information from third party news sources. Also we would like to give users the ability to discuss news topics that may have not been highlighted on our platform.

## Product Spec

1. **User Stories (Required and Optional)**
**Required Must-have Stories**
- User logs in to have the ability to participate in chats and see news 
- users are able to choose what tyoe of news they would like to see or it would categorized for them to search through
- Settings (accessibility, notifcations, General, etc.)
**Optional Nice-to-have Stories**
- Choose what type of news topics they want to see
- User are able to see chats that have particpated in
- see most popular chats and most popoular news 

2. **Screens**
- Login
- Category Screen
- Chats screeen
- Feed/Home Screen
- News Article Screen
- Settings Screen

3. **Navigation**

**Tab Navigation** (Tab to Screen)
- Home
- chats 
- settings 

Optional:
- Top choices
- participated chats

**Flow Navigation** (Screen to screen)
- Forced Log-in
- Category Page -> shows feed based on selection
- Profile page -> Settings page 

## Wireframes

![wireframe drawing](https://user-images.githubusercontent.com/89495809/140865964-6fd7258f-c507-46c3-9da0-1863f55a4164.jpeg)

**Digital Wireframes & Mockups**

<img width="408" alt="Screen Shot 2021-11-09 at 5 35 32 PM" src="https://user-images.githubusercontent.com/89495809/141016702-b3dc7362-a5da-461a-b2b4-194d01006b98.png">

**Interactive Prototype**

https://user-images.githubusercontent.com/89495809/141018060-1ca9a27e-2c52-47a6-a26d-5e8095c2d707.mov

## Schema
**Models**

User
| Property | Type | Description |
| ----------- | ----------- | ----------- |
| username | String | unique id for the user and a way to login |
| firstName | String | user first name |
| lastName | String | user last name |
| email | String | a way for user to get notifications |
| password | String | A way for user to login |
| image | File | image of the user |

Chats
| Property | Type | Description |
| ----------- | ----------- | ----------- |
| objectId | String | unique id for the user and a way to login |
| author | Pointer to user | user image and username |
| title | String | title of the chat|
| content | String | what the users post |
| createdAt | DateTime | when the chat started |

Comments
| Property | Type | Description |
| ----------- | ----------- | ----------- |
| objectId | String | unique id for the user and a way to login |
| author | Pointer to user | user image and username |
| content | String | what the users post |
| likeCount | Number | amount of like a comment get |
| createdAt | DateTime | Date when the comment started |
