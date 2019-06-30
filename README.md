# Web Chatting App
This is a learning roadmap for a simple `single-page application` for chatting.
It includes project base and future corrections and will help you to take some experience in developing.
**It's important to go over corrections strictly in order and exactly meet the requirements.**

Any `code` quote is ready for google and research it. (But please, dont copy code)

This project does not include any concrete steps, because with steps it will be repeating guide.
Main goal of this project is help you to take close to real developing experience.

## Frontend
- Written on `JS`
- Bundled with `rollup`
- Created using `vue.js`
- Desktop version only
- There are two pages:
  1. Login page (nick entering)
  2. Chat page (one chat for all)
     - Messages log with nicknames
     - Message input field and send button

## Backend
- Based on `node.js`
- Used `WebSockets` for communication

## Correction #1
- Lets protect user accounts: now there is a `password authentication`
  - Verify credentials, if nickname is new, than create user
  - Store credentials in `sqlite` database

## Correction #2
- Messages log is not comfortable now, lets redesign it
  - Display remote messages on the left, local on the right
  - Message `background color` based on nickname

## Correction #3
- Oh no, I refreshed page and messages disappears, lets save them
  - Save messages into the `sqlite` database
  - Load them on start

## Correction #4
- As it is quite bored in this chat, lets add memes:
  - Add `image uploading` and sending
  - Add emoji selection menu

## Correction #5
- My friend wants to join the chat, but I have old private romantic messages there:
  - Do not show old messages for new users
  - Add ability to delete messages

## Correction #6
- That stupid friend is unable to start local server with app, lets host it in the world:
  - Reorganise project for running on `heroku`
  - And run it on free server

## Correction #7
- Oh no, all messages were disappeared, because `heroku` not stores local files:
  - Add any database add-on on `heroku`
  - And migrate app to it
- Images are also local?
  - Just store them somewhere

## Correction #8
- Finally, the friend decided to yell with memes:
  - Add discord-like reactions for images
  - Without any protection, just like images with an emoji

## Correction #9
- There are so many messages that they are loading endless:
  - Modify messages loading to blocks mode (on scrolling)
