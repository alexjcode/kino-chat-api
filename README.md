# Kino Chat

Front-end [ [Repo](https://github.com/alexjcode/kino-chat) / [Deployed](https://alexjcode.github.io/kino-chat) ]

Back-end [ [Repo](https://github.com/alexjcode/kino-chat-api) / [Deployed](https://kino-chat-api-55523.herokuapp.com) ]
​
## Summary
A simple chat app where users can discuss films and shows that they're watching online. Netflix doesn't have any sort of comment section or forum, so this is meant to fill that need.

## Getting Started
- Click the `Sign Up` button at the top of the page to make an account
- Fill in an email and password `don't use a password that you use on other sites` and click submit
- You're now signed in! Go ahead and chat with the group by adding new messages.
- If you made a mistake, either click the message to edit, or click the `x` button to delete your message
​
## Technologies used
- Node.js
- React.js
- Javascript
- Socket.io
- Express
- MongoDB
- Mongoose
- Webpack
- React-Bootstrap
- Git
- GitHub

## Setup Back End
- `git clone` this repo
- `cd` into its directory
- `npm install`
- `npm run server`

## Planning
- Create both repos
- Deploy
- Create a basic API, with users and messages owned by the users
- Figure out how to use Socket.io with React and API
- Complete the Front End functionality using React and Socket.io

## Process
Most of the project consisted of me learning Socket, and learning how to use React correctly. The rest was very straightforward, especially the API.
​
## Problem Solving Strategy
The biggest bump in the road was not knowing how use Socket.io, and that along with Reatc took me about 2 days to figure out.
To figure out Socket and React, I was quicker about making issues in the issue queue, I watched YouTube videos, I looked at the docs, at StackOverflow, FreeCodeCamp, Medium, and anything else I could find. Many of the smaller bugs I encountered were misspelling or mislabeling of elements.
​
## ERD
<img src="https://i.imgur.com/eLV9gn2.jpg" width="100%" alt="ERD">

## API Routes
| Verb   | URI Pattern        | Request Body      | Headers   | Action              |
|--------|--------------------|-------------------|-----------|---------------------|
| POST   | `/sign-up`         | **credentials**   | N/A       | user sign-up        |
| POST   | `/sign-in`         | **credentials**   | N/A       | user sign-in        |
| DELETE | `/sign-out`        | N/A               | **Token** | user sign-out       |
| PATCH  | `/change-password` | **passwords**     | **Token** | change-password     |
|        |                    |                   |           |                     |
| GET    | `/posts`           | N/A               | N/A       | index posts         |
| GET    | `/posts/:id`       | N/A               | N/A       | show single post    |
| POST   | `/posts`           | `post: {}`        | **Token** | create post         |
| PATCH  | `/posts/:id`       | post              | **Token** | update post         |
| DELETE | `/posts/:id`       | N/A               | **Token** | remove post         |

## Unsolved Problems
- Needs Styling
- Profile pictures
- Allow for users to join different channels in a chat room.
- Anti-spam filtering
- Search for channels
- **FilmTalk: Channels are centered around episodes of shows or films. Chat with others while watching your favorite shows. Uses a 3rd party API.
