# Notes App

[Project Description](#project-description) | [Tech Stack](#tech-stack) | [Installation](#installation) | [Running tests](#running-tests) | [Development Process](#development-process) | [User Stories](#user-stories) | [Models](#models) | [Approach](#approach) | [Further development](#further-development)

## Project Description

`Challenge:` Build a frontend, single page web app to create and list notes

### The Team:

Project created by the team: ([Ed Ancerys](https://github.com/EdAncerys), [Dec Kolakowski](https://github.com/dpwdec), [Catriona Bennett](https://github.com/cmb84scd), [Marija Trachtenberg](https://github.com/Tracht), ) at Makers Academy.

## What we done

- Our app allows user to add and save notes
- User able to preview notes in shorten format
- User able to navigate to note added by clicking a link

## Tech Stack:

- [Custom Test Framework](#) Testing framework developed while coding at Makers academy. Inspired by [Jasmine](https://jasmine.github.io/).

## Installation

- Clone this repository
  `$ git clone https://github.com/EdAncerys/Notes-App`
- Navigate to local repository
  `$ cd Notes-App`
- Open index.html
  `$ open index.html`

## Running tests

- Navigate to local repository
  `$ cd Notes-App`
- Open SpecRunner.html
  `$ open SpecRunner.html`

## Development Process

Our team used an agile development process with regular sprints to deliver this application.
We followed the Extreme Programming values - all features were pair programmed, team members shared all the changes in the code design, the team used test-driven development, and delivered an MVP in the first sprint.
During development we used an agile process of git branches, merges, regular code reviews, and continuous integration.
We had daily stand-ups and retrospectives to update each other on the tasks completed, and reflect on our team's progress.

## Models

| Object | Message   |
| ------ | --------- |
| Note   | body()    |
|        | preview() |

| Object      | Message         |
| ----------- | --------------- |
| NoteManager | numberOfNotes() |
|             | addNote()       |
|             | getNote(index)  |

## User Stories

```
As a programmer
I can see a list of my notes, where each note is abbreviated to the first 20 characters
So I can find the one I want

As a programmer
I can create a new note
So I can record something I need to remember

As a programmer
I can see the full text of an individual note on its own page
So I can see all the information in the note
```

## Approach

View notes 20 characters each

- [x] object that holds notes
- [x] instantiate notes
- [x] retrieve list of notes
- [x] note function that returns first 20 characters of the note body
- [x] a way to get those 20 characters onto the page as an element
- [x] create a list of HTML elements as links on the page
- [x] updates every time new note is added

Create a note

- [x] generate text box element
- [x] generate a submit button
- [x] get text from text box and put it into a element on the page
- [x] new note object
- [x] clear text element box when note is generated
- [x] stop empty notes being added

Create note Manager

- [x] holds an array of note objects
- [x] create addNote method to add note objects to array
- [x] create getNote method to retrieve a note

View full note

- [x] clicking link suppresses default event and triggers custom event
- [x] retrieve particular note's full text
- [x] generate HTML element that holds full note text

## App UI Preview

<img width="280" alt="homepage" src="https://user-images.githubusercontent.com/28805811/83274013-1b7c9480-a1c5-11ea-9d72-84f5b63598bd.png">

<img width="273" alt="fullNotePage" src="https://user-images.githubusercontent.com/28805811/83274015-1c152b00-a1c5-11ea-804a-58badf24ed90.png">

## Further Development

Ideas to improve our application

- Add feature to add note description
- Add feature to save notes to DB
- Improve UI and consider to develop it in React or/and Bootstrap
