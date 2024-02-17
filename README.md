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

### User Story 1
Story ID: User-01

#### User Story Statement

As a new user, I want to be able to register for an account.

#### Criteria
- Users should be able to register an account easily, preferable with minimal information
- Users should be sent a confirmation link via email, to confirm that they are the owner of the email account

#### Dependencies
- Creating a sign up/create account landing page for users
- Implement a automatated email to provided user email account, that activates the account when clicked
- Register and Authentication routes in Backend

### User Story 2
Story ID: User-02

#### User Story Statement

As a registered user, I want to be able to log in securely to access the app's features.

#### Criteria
- Authentication mechanisms should be secure to prevent unauthorised access.

#### Dependencies
- Implement password hashing and encryption, JWT
- Login Route, encryption, decryption, checking

### User Story 3
Story ID: User-03

#### User Story Statement
As a registered user, I want the option to reset my password if I forget it.

#### Criteria
- Users should have the ability to manage their account settings, updating email address, password

#### Dependencies
- Create a user account settings page that enables them to change their settings
- Update route for users, authentication / authorisation to update

### User Story 4
Story ID: User-04

#### User Story Statement
As a user I want to be able to browse through various posts and game pages

#### Criteria
- Intuitive Navigation
- Users should be able to View Posts by Community, Posts by Friends etc.

#### Dependencies
- News and Community Game Pages, ability to follow communities, Timelines of Shared Friends Content
- Community CRUD routes in backend
- Follow and Unfollow routes
- Post CRUD routes

### User Story 5
Story ID: User-05

#### User Story Statement
As a user I want to be able filter posts and sort posts based on criteria

#### Criteria
- Efficient Filtering and Sorting Options
- API support for queries

#### Dependencies
- Read routes with Query Parameters for Sorting, Filtering Posts
- Posts CRUD implemented
- Front end form elements for modifying query parameters

### User Story 6
Story ID: User-06

#### User Story Statement
As a user I want to be able to view posts, content, and media attachments

#### Criteria
- Clear Presentation of Post Titles, Content, and Media
- Embedded / Uploaded Media

#### Dependencies
- Post CRUD
- Embedded content support in backend
- Links to hosted media saved in post
- Viewing posts should display supported content correctly

### User Story 7
Story ID: User-07

#### User Story Statement
As a user I want to be able to create new posts in specfic game pages

#### Criteria
- User friendly post creation interface
- Posts are associated with Users, and specific game pages

#### Dependencies
- Game Pages CRUD implemented
- Game Page View implemented
- Posts CRUD implemented
- Create Route takes user and game into account
- Front end form for creating a new post on the game page

### User Story 8
Story ID: User-08

#### User Story Statement
As a user I want to be able to include text, images and links in the posts I create

#### Criteria
- Support for text, images, links and media attachments

#### Dependencies
- As User Story 6, plus
- Support for embedded links and images, data saved in API, including links to images
- Create post form support for inserting links, images, media attachments

### User Story 9
Story ID: User-09

#### User Story Statement
As a user I want to be able to edit and delete my own posts.

#### Criteria
- User ability to edit and delete posts
- Security to ensure users can only delete their posts
- Game admins can delete posts

#### Dependencies
- Post CRUD
- Authentication / Authorisation to determine who can edit/delete posts
- Front end buttons / forms to edit and delete posts (if different from creating posts)

### User Story 10
Story ID: User-10

#### User Story Statement
As a user I want to be able to react to posts, like or emoji reactions

#### Criteria
- Visual indicators for reacted content
- Real time react count updates
- Support various emojis

#### Dependencies
- Posts CRUD
- User Authentication
- Reactions CRUD and backend
- Front end support for various reacts
- WebSocket for count updates.

### User Story 11
Story ID: User-11

#### User Story Statement
As a user I want to be able share posts to friends

#### Criteria
- Users should be able to share posts to their friends within the app
- Users should be able to share posts outside of the app

#### Dependencies
- Create a share button on each post, that will allow you to share the post internally and externally

### User Story 12
Story ID: User-12

#### User Story Statement
As a user I want to be able follow specfic games, to help customise my feed

#### Criteria
- Users should be able to follow and unfollow games when they want
- Users should be able manage the games they follow

#### Dependencies
- Create a follow button on a games page
- Follow button will toggle whether or not you see posts from that game in your feed
- Create a page that lists all the games that you've followed

### User Story 13
Story ID: User-13

#### User Story Statement
As a user I want to be able to join discussions by commenting on posts

#### Criteria
- User ability to interacte with post
- User ability to comment on posts/join discussion

#### Dependencies
- Create a comment button for posts
- Create a page that shows all comments for the post

### User Story 14
Story ID: User-14

#### User Story Statement
As a user I want to be able recieve notifications for replies from posts, important updates from games and friend requests

#### Criteria
- A user should be able to easily see they have new notifications
- The user should be able to quickly see notifications from their timeline page
- There should also be a way to view the notifications as its own page

#### Dependencies
- Create a notification icon that shows that you have new notifications
- Create a way to interact with that icon but doesn't obstructu user navigation
- Create a seperate way to view all notifications

### User Story 15
Story ID: User-15

#### User Story Statement
As a developer, I want to be able to create and manage a page for my game

#### Criteria
- Developer account should be able to create, edit and delete a game page
- Create posts for that page
- Moderate comments and community posts

#### Dependencies
- Implement a developer user with special privileges
- Create a way for a user to be assigned as a developer

### User Story 16
Story ID: User-16

#### User Story Statement
As a moderator, I want to be able to manage posts and comments within my assigned game page.

#### Criteria
- A developer should be able to assign a user as a moderator for their game

#### Dependencies
- Implement a way for a developer to assign moderator privileges to a user
- Give moderators privileges to manage post, comments (remove spam, ban users, respond to posts)

### User Story 17
Story ID: User-17

#### User Story Statement
As an administrator, I want to have the ability to manage overall site settings, user accounts, and reported content

#### Criteria
- User accounts should be able to be assigned as an admin account
- Admin account should be able to manage user accounts, site settings and reported content effectively

#### Dependencies
- Implement an admin user with special privileges
- Create a way for a user to get assigned as an admin

### User Story 18
Story ID: User-18

#### User Story Statement
As a user I want the website to be responsive and accessible across multiple different devices

#### Criteria
- User should be able to access website from multiple difference devices
- The layout/accessbility shouldnt break between screen size differences

#### Dependencies
- Implement css media queries for varying sizes of screens
- Use response viewport units so website scales according to device screen size

### User Story 19
Story ID: User-19

#### User Story Statement
As a user I want the app to have clear navigation and intuitive UI elements for ease of use

#### Criteria
- Users should be able to access most navigation items from the timeline page

#### Dependencies
- Ensure that navigation is intuitive and easily accessible from any point within the app

### User Story 20
Story ID: User-20

#### User Story Statement
As a user I want to be able to search for posts, games or users

#### Criteria
- Users should have access to a search function

#### Dependencies
- Create a search bar that searchs through matching user names, games and relevant posts
- Create contectual search bar, i.e. search bar within friends page only searchs users
- Auto suggestions for search queries


### User Story 21
Story ID: User-21

#### User Story Statement
As a user I want to be able to discover new games or trending topics based on my interests

#### Criteria
- User should be able to discover new games or topics with ease

#### Dependencies
- Create a page that shows a list of games within the database app
- Create filters to better refine discoverability

### User Story Revision History

#### Version 1:
Our initial user stories were more broad and ecompassing many features, see below for examples

User Story Statement 1:

As a Game Developer, I want to implement a community page for my game to build interest and awareness before the launch, so that more people will be excited about and aware of my game.

User Story Statement 2:

As a Community Manager, I want to be able to give feedback and updates to players quickly, so that they kept up to date with important information

User Story Statement 3:

As a User, I want to be able to browse, interact, follow and discover my favourite games, whilst also being able to feel a part of a community within each game.

#### Version 2: 
We further broke down user stories into many more smaller experiences, to help better identify criteria and dependencies. This lead us to have 21 User Stories

---

## Wireframes

### Timeline Page

#### News Timeline
![Desktop News Timeline](/docs/web-timeline-news.png)
![Mobile News Timeline](/docs/mobile-news-timeline.png)

#### Community Timeline
![Desktop Community Timeline](/docs/web-timeline-community.png)
![Mobile Community Timeline](/docs/mobile-timeline-community.png)

### Game Landing Page

#### Game News
![Desktop Game News Page](/docs/web-game-news-timeline.png)
![Mobile Game News Page](/docs/mobile-game-news-timeline.png)

#### Game Community
![Desktop Game Community Page](/docs/web-game-community-timeline.png)
![Mobile Game Community Page](/docs/mobile-game-community-timeline.png)

#### Game About
![Desktop Game About Page](/docs/web-game-about.png)
![Mobile Game About Page](/docs/mobile-game-about.png)

### Explore page

![Desktop Explore Page](/docs/web-explore.png)
![Mobile Explore Page](/docs/mobile-explore.png)

### Chats page
![Desktop Chat](/docs/web-chat.png)
![Mobile Chat](/docs/mobile-chat.png)

### Friends
![Desktop Friends](/docs/web-friends.png)
![Mobile Friends](/docs/mobile-friends.png)

### Notifications
![Desktop Notifications](/docs/web-notifications.png)
![Mobile Notifications](/docs/mobile-notifications.png)

### Settings

#### Account Settings
![Desktop Account Settings](/docs/web-user-account-settings.png)
![Mobile Account Settings](/docs/mobile-user-account-settings.png)

#### Profile Settings
![Desktop Profile Settings](/docs/web-user-profile-settings.png)
![Mobile Profile Settings](/docs/mobile-user-profile-settings.png)

### Sidebar Navigation

#### Friends
![Desktop Sidebar Friends](/docs/web-sidebar-nav-friends.png)
#### Chat
![Desktop Sidebar Chat](/docs/web-sidebar-nav-chat.png)
#### Notification
![Desktop Sidebar Notifications](/docs/web-sidebar-nav-notifications.png)

### Posting

#### Create a Post
![Desktop Create a Post](/docs/web-create-post.png)
![Mobile Create a Post](/docs/mobile-create-post.png)

#### Comment on a post
![Desktop Comment on a Post](/docs/web-comment-on-post.png)
![Mobile Comment on a Post](/docs/mobile-comment-on-post.png)


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

### 15th Feb, 2024

![Trello Screenshot](/docs/trello11.png)

### 16th Feb, 2024

![Trello Screenshot](/docs/trello12.png)

