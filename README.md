# t3a2-a-full-stack-app-part-a
Readme file for Part A of final Coder Academy project, designing and planning a Full Stack MERN App

## Description of the website:

Video Game Community Social Media App
- Think subreddit for games, a community specific to video game discussion (or video game development?)
- Social Media for video game communities or forums
- Maybe posts are always tied to a specific game (with tags)


## Purpose

Social Gaming Forum app

There are currently a lot platforms for video game engagment, this aiming to solve that be being single social platform to for gaming enthuiasts to chat, be informed and connect. The aim is to provide a platform for gamers to conntect, chat, share content, follow gaming news, updates and explore new games.

### Minimum Viable Product
- Realtime Chat
  - Private Messaging option between users
- User creation, login, authentication, profile
  - Follow game communities
  - Add friends
- User timeline
  - View posts from followed communities
- Game community pages
  - Posts
  - Comments

### Extended Features
- User creation wiht OAuth
- Group Chat
  - Private messaging between a group of users
- Timeline
  - Share post from communities, friends will see the shared post in their timeline
  - Like posts from communities
- Explore feature
  - explore games that you don't follow
- Embedded Media (Videos / pictures)

## Functionality / features

- User Registration and Login
- User Authentication
- User Profile editing
  - account settings
  - Profile picture

- Chat
  - Private Messaging option between users
  - Users can create a group for multiple users to chat
  - Send and receive media in chat such as photos, videos or documents
  - Encryption of messages
  - Indicators to know the status of a sent message (read, received)
  - Push notification alerts
  - Emoji support
  - Gif integration
  - Clickable links
  - React to messages

- Explore page
  - list of a galley of game pages to follow

- User Upload and View Content
  - Videos
  - Embed Youtube Videos
  - Pictures
  - Comments

- Game manager upload content
  - videos
  - posts

- User Timeline Feed
  - posts from communities you are in / follow
  - shared posts from friends
 

- User-Created Public Pages ?
    - (are user created public pages tied to a game)
  - Messages / Public Posts ?
  - Support for various forms of content as above
  - Admin powers for kick, ban, approve users
 

## Target audience
- Gamers
- Game developers
- Content Creators / Streamers
- Anyone interested in Games, Game Development or Game-related content

## Tech stack
- MERN:
  - MongoDB
  - Express.js
  - React
  - Node.js
- Packages:
  - dot-env
  - mongoose
  - express
  - react
  - (Socket?)
  - Encryption:
    - bcrypt
    - cors
    - helmet
    - jsonwebtoken
  - Dev Dependencies:
    - nodemon
    - jest
- External APIs:
  - ...


## Application Architecture Diagram

The below diagram outlines the architecture of this application:

![Social Gaming Forum Application architecture](/docs/ApplicationArchitectureDiagram.png)

## Data Flow Diagrams

The below diagrams show the flow of data of the application: 

![Data Flow](/docs/DataFlow.png)

## User Stories

*User Registration and Authentication*

### User Story 1
Story ID: User-01

#### User Story Statement

As a new user, I want to be able to register for an account.

#### Criteria
- Users should be able to register an account easily, preferable with minimal information
- Users should be sent a confirmation link via email, to confirm that they are the owner of the email account

#### Dependencies
- Creating a sign up/create account landing page for users
- Implement a automatication sent email to provided user email account, that activates the account when clicked

#### Revision History for User-01
Version 1: ...

### User Story 2
Story ID: User-02

#### User Story Statement

As a registered user, I want to be able to log in securely to access the app's features.

#### Criteria
- Authentication mechanisms should be secure to prevent unauthorised access.

#### Dependencies
- Implement password hashing and encryption

#### Revision History for User-02

### User Story 3
Story ID: User-03

#### User Story Statement
As a registered user, I want the option to reset my password if I forget it.

#### Criteria
- Users should have the ability to manage their account settings, updating email address, password

#### Dependencies
- Create a user account settings page that enables them to change their settings

#### Revision History for User-03

*Browsing Content*

### User Story 4
Story ID: User-04

#### User Story Statement
As a user I want to be able to browse through various posts and game pages

#### Criteria
- Intuitive Navigation

#### Dependencies

#### Revision History for User-04
Version 1: ...

### User Story 5
Story ID: User-05

#### User Story Statement
As a user I want to be able filter posts and sort posts based on criteria

#### Criteria
- Efficient Filtering and Sorting Options

#### Dependencies

#### Revision History for User-05
Version 1: ...

### User Story 6
Story ID: User-06

#### User Story Statement
As a user I want to be able to view posts, content, and media attachments

#### Criteria
- Clear Presentation of Post Titles, Content, and Media

#### Dependencies

#### Revision History for User-06
Version 1: ...

*Content Creation*

### User Story 7
Story ID: User-07

#### User Story Statement
As a user I want to be able create new posts in specfic game pages

#### Criteria
- User friendly post creation interface

#### Dependencies

#### Revision History for User-07
Version 1: ...

### User Story 8
Story ID: User-08

#### User Story Statement
As a user I want to be able to include text, images and links in the posts I create

#### Criteria
- Support for text, images, liks and media attachements
#### Dependencies

#### Revision History for User-08
Version 1: ...

### User Story 9
Story ID: User-09

#### User Story Statement
As a user I want to be able edit and delete my own posts.

#### Criteria
- User ability to edit and delete posts

#### Dependencies

#### Revision History for User-09
Version 1: ...

*Interacting with content*

### User Story 10
Story ID: User-10

#### User Story Statement
As a user I want to be able react to posts, like or emoji reactions

#### Criteria
- Visual indicators for reactted content
- Real time react count updates

#### Dependencies

#### Revision History for User-10
Version 1: ...

### User Story 11
Story ID: User-11

#### User Story Statement
As a user I want to be able share posts to friends

#### Criteria
- Share post feature

#### Dependencies

#### Revision History for User-11
Version 1: ...

*Community Engagment*

### User Story 12
Story ID: User-12

#### User Story Statement
As a user I want to be able follow specfic games, to customise my feed

#### Criteria
- Game subscription/follow management

#### Dependencies

#### Revision History for User-12
Version 1: ...

### User Story 13
Story ID: User-13

#### User Story Statement
As a user I want to be able to join discussions by commenting on posts.

#### Criteria
- User ability to comment on posts/join discussion

#### Dependencies

#### Revision History for User-13
Version 1: ...

### User Story 14
Story ID: User-14

#### User Story Statement
As a user I want to be able recieve notifications for replies from posts, and important updates from games

#### Criteria
- Notification feature for replies and updates from games

#### Dependencies

#### Revision History for User-14
Version 1: ...

*Moderation and Administration*

### User Story 15
Story ID: User-15

#### User Story Statement
As a developer, I want to be able to create a page for my game

#### Criteria
- Tools to allow

#### Dependencies

#### Revision History for User-15
Version 1: ...

### User Story 16
Story ID: User-16

#### User Story Statement
As a moderator, I want to be able to manage posts and comments within my game page.

#### Criteria

#### Dependencies

#### Revision History for User-16
Version 1: ...


### User Story 17
Story ID: User-17

#### User Story Statement
As an administrator, I want to have the ability to manage overall site settings, user accounts, and reported content

#### Criteria

#### Dependencies

#### Revision History for User-17
Version 1: ...

*Accessibility and Usability*

### User Story 18
Story ID: User-18

#### User Story Statement
As a user I want the website to be responsive and accessible across multiple different devices

#### Criteria

#### Dependencies

#### Revision History for User-18
Version 1: ...


### User Story 19
Story ID: User-19

#### User Story Statement
As a user I want the app to have clear navigation and intuitive UI elements for ease of use

#### Criteria

#### Dependencies

#### Revision History for User-19
Version 1: ...

*Search*

### User Story 20
Story ID: User-20

#### User Story Statement
As a user I want to be able to search for posts, games or users

#### Criteria
- Create a search bar that searchs through matching user names, games and relevant posts

#### Dependencies

#### Revision History for User-20
Version 1: ...

### User Story 21
Story ID: User-21

#### User Story Statement
As a user I want to be able to discover new games or trending topics based on my interests

#### Criteria
- Create an explore page that shows trending content, and content that share tags with the games you follow
 
#### Dependencies

#### Revision History for User-21
Version 1: ...

### User Story 22
Story ID: User-22

#### User Story Statement
As a user I want to be able to discover new games or trending topics based on my interests

#### Criteria
- Create an explore page that shows trending content, and content that share tags with the games you follow
 
#### Dependencies

#### Revision History for User-22
Version 1: ...

---

#### Story ID 
User-0

#### User Story Statement
As a Game Developer, I want to implement a community page for my game to build interest and awareness before the launch, so that more people will be excited about and aware of my game.

#### Criteria
- Ability to create a responsive landing page accessible from various devices.
- Include a brief game description, and key features.
- Implement social media sharing buttons for easy sharing.
- Provide a "Follow" button for users to receive post notifications
- Ability to post videos, concept art, screenshots.

#### Dependencies

Identify any dependencies or prerequisites required for implementing the user story.

#### Revision History for User-0:
Version 1: Initial story

Version 2: Updated because of “something” etc

Version 3: Revised to include a function after testing etc

### User 3

#### User Story Statment
As a Community Manager, I want to be able to give feedback and updates to players quickly, so that they kept up to date with important information

#### Criteria

---

## Wireframes for multiple standard screen sizes, created using industry standard software

Start thinking about the different pages to include for wire frames

- Timeline Page
- Explore Page
- Game landing Page
- Group Community Page
- Profile Page

## Screenshots of your Trello board throughout the duration of the project

