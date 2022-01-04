# React Project: Memory Card

And here we go again with a new project! Let’s make sure you understand the concepts so far. The main goal of this project should be to use lifecycle methods, as props and state.

## Repo Link: React [Memory Game Project](https://github.com/Bryantellius/react_memorygame_project)

## How The Game Works

Go play around [here](https://complete-memory-game.herokuapp.com/) to get a feel for the goal of this project. Your objective is to create a game that displays items to the screen. The game tests the user’s memory. The user clicks the items on the screen, making sure to select an item that they have not previously selected. Your application should know if they have, or have not clicked a certain item. If they select an item that they previously selected, the game starts over, and their best score is saved.

Also, make sure to randomize the items on screen after each selection. We don’t want the game to be too easy.

Also, you can use any collection of items that you want. I used numbers 1-10 in Japanese, but you can use numbers, words, pictures, etc.

## Getting Started

- Open your command line and navigate to your repos directory (if you do not have a repos folder, then you can use mkdir repos to create one)
- Use this template repository to start a new project in your repos folder: git clone &lt;repo_name> cd repo_name to navigate into your new repo directory
- Make sure to run npm install to fetch the dependencies for the project
- Start Visual Studio Code and select 'Open Folder'. Then select repo_name to open the folder in the editor (or just type code . in your terminal inside the repo directory)
- Follow the instructions on the README.md file to complete exercises
- Open the app.js file to get started

## Project

- View this working example to see the end goal: [Memory Game](https://complete-memory-game.herokuapp.com/)
- Take a little bit of time to think about how you want to implement your application, the features you want to implement, which components you need, and how to structure your application.
- You can choose to replicate with numbers, or any other group of items (e.g. images, colors, words)
  1. Your application should include:
- Cards with the memory items, a scoreboard, which counts the current score, and a best score, which shows the best score you achieved thus far.
  1. You also need a couple of cards that display images and possibly informational text. There should be a function that displays the cards in a random order anytime a user clicks one. Be sure to invoke that function when the component mounts.
  2. So now that you thought about the structure of your application, set up the folder structure, and start creating the class components.
  3. Style your application so you can show it off!
  4. As always, push the project to GitHub.
- First, build this project with class components. Once you complete the project, you have the option of rewriting the class components as functional components with react hooks.

<br>