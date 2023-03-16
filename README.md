# The Odin Project - Todo List

This is a solution to the [ToDo Project from The Odin Project](https://www.).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- view all projects
- view all todo's in each project (probably just the title and due date... perhaps changing color for different priorities)
- expand a single todo to see/edit its details
- delete a todo

### Screenshot

![Screenshot](./screenshot.png)

### Links

- Solution URL: []()
- Live Site URL: []()

## My process

Each 'todo' will be an object that is created dynamically.
So either factories or constructors/classes.

What properties should they have?

- title
- description
- dueDate
- priority
- notes
- checklist

The todo list should have `projects` or separate lists of `todos`.
When a user first opens the app, there should be a 'default' project to which all their todos are put.

Users should be able to create new projects and choose which projects their todos go into.

Keep application logic (creating new todos, setting todos as complete, changing todo priority) from the DOM-related stuff.

Add some persistence with the Web Storage API (`localStorage`)

---

Steps:

- I decided to create the app wholly in the console at the beginning to ensure decoupling of the logic from the DOM-related stuff.

- Setting up a local environment with npm for webpack and set up the configuration.

- A project is a collection of `todos`

  - A default project before user creates any

- A todo is an object
  - title
  - description
  - dueDate
  - priority

Use a factory function to create todos, since there will be multiple created.

- Something like:

  ```js
  const Todo = (title, description, dueDate, priority) => {};
  ```

- Or maybe a class:

  ```js
  class Todo {
    constructor(title, description, dueDate, priority) {}
  }
  ```

I decided to go with a factory function for the private methods and fields.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- SCSS
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

### Continued development

### Useful resources

## Author

- Website - [Nathaniel Adiah](https://nathanieladiah.github.io)
- Frontend Mentor - [@nathanieladiah](https://www.frontendmentor.io/profile/nathanieladiah)
- Twitter - [@nathanieladiah](https://www.twitter.com/nathanieladiah)
