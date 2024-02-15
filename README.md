# t3a2-a-full-stack-app-part-a
Part A of a Coder Academy final project, designing and planning a Full Stack MERN App

## Website Description

A Video Game Social Platform that features User Chat, Posts, and Profile features, along with Game News, Updates and Communities.

### Purpose

There are currently a lot of platforms for video game engagement which offer different combinations of features, but do not provide a single platform for game news, communities and chat. This aims to solve that be being the single social platform for gaming enthuiasts to chat, be informed and connect. The aim is to provide a platform for gamers to connect, chat, share content, follow gaming news, updates and explore new games.

### Functionality / Features

#### Minimum Viable Product
- Event-driven Chat (WebSocket)
  - Private Messaging option between users
- User creation, login, authentication, profile
  - Follow game communities
  - Add friends
- User timeline
  - View posts from followed communities
- Game community pages
  - Posts
  - Comments

#### Extended Features
- User creation with OAuth
- Timeline
  - Share post from communities, friends will see the shared post in their timeline
  - Like posts from communities
- Explore feature
  - explore games that you don't follow
- Embedded Media (Videos / pictures)
- Message / User / Typing status indicators for chat
- Chat
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
  - Trending or suggested games listed
- User Upload and View Content
  - Videos
  - Embed Youtube Videos
  - Pictures
- Game manager uploaded content
  - Posts
  - Videos
- User Timeline Feed
  - Shared posts from friends
 - User-Created Community pages
    - User created public pages tied to a game
    - Posts
    - Support for various forms of content as above
    - Admin powers for kick, ban, approve users
 

### Target Audience
- Gamers
- Game Developers
- Content Creators / Streamers
- Anyone interested in Games, Game Development or Game-related content

### Tech stack
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
  - Encryption:
    - bcrypt
    - cors
    - helmet
    - jsonwebtoken
  - Dev Dependencies:
    - nodemon
    - jest
- External APIs:
  - WebSocket
  - OAuth


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

### Timeline Page

#### Desktop
![Desktop News Timeline](/docs/web-timeline-news.png)
![Desktop Community Timeline](/docs/web-timeline-community.png)

#### Mobile
![Mobile News Timeline](/docs/mobile-news-timeline.png)
![Mobile Community Timeline](/docs/mobile-timeline-community.png)

### Explore page

#### Desktop
![Desktop Explore Page](/docs/web-explore.png)

#### Mobile
![Mobile Explore Page](/docs/mobile-explore.png)

### Game Landing Page

#### Desktop
![Game News Page](/docs/web-game-news-timeline.png)
![Game Community Page](/docs/web-game-community-timeline.png)
![Game About Page](/docs/web-game-about.png.png)

#### Mobile
![Game News Page](/docs/mobile-explore.png)

### Game Landing Page
#### Desktop
#### Mobile
- Game landing Page
- Group Community Page
- Profile Page



## Trello Board Screenshots
The Trello Board used for this project is available [here](https://trello.com/invite/b/nAU98IPU/ATTIf939cd062b458d6c45c964efc5ffb3ee12208611/chatclient).

### 28th Jan, 2024
![Trello Screenshot](/docs/trello00.png)

![Trello Screenshot](/docs/trello01.png)

![Trello Screenshot](/docs/trello02.png)

### 29th Jan, 2024

![Trello Screenshot](/docs/trello03.png)

### 30th Jan, 2024

![Trello Screenshot](/docs/trello04.png)

### 1st Feb, 2024

![Trello Screenshot](/docs/trello05.png)

### 4th Feb, 2024

![Trello Screenshot](/docs/trello06.png)

### 9th Feb, 2024

![Trello Screenshot](/docs/trello07.png)

![Trello Screenshot](/docs/trello08.png)

### 13th Feb, 2024

![Trello Screenshot](/docs/trello09.png)

### 14th Feb, 2024

![Trello Screenshot](/docs/trello10.png)
