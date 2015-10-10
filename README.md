# todo-tracker
A meteor app that checks your codebase for TODO's 

## Elevator Pitch
For developers…
…who want to keep track of the todos in their codebase…
…Todo Tracker…
…is a todo tracker…
…that automagically creates trello cards for the todos in your codebase…
…unlike other todo trackers…
…it is open source and just works…

## Feature Stories
**Feature:** list todos from github repos
  In order to keep track of my todos
  As a meteorite I want to see a list of my todos

  **Scenario:** log in with github
    **Given** I am not logged in
    **When** I click on ‘log in with github
    **And** I fill in ‘username’ with my username
    **And** I fill in ‘password with my password
    **Then** I should see ‘Add repo’

  **Scenario:** add repo
    **Given** I am logged in
    **When** I click on ‘Add repo’
    **And** I fill in ‘Owner name’ with the owner name
    **And** I fill in ‘Repo name’ with a repo name
    **Then** I should see ‘Repo name’

  **Scenario:** view repo
    **Given** there is a repo
    **When** I click on ‘Repo name’
    **Then** I should see ’Todo 1’

  **Scenario:** remove repo
    **Given** there is a repo
    **When** I click on ‘Delete repo’
    **Then** I should see ‘You have not yet added any repos’

**Feature:** cli
  In order to work comfortably from within the terminal
  As a meteorite I want to use a cli

**Feature:** daily recap
  In order to keep track of my todos at all times
  As a meteorite I want to receive recaps via email on a daily basis

**Feature:** trello integration
  In order to work with the kanban technique
  As a meteorite I want to see my todos as trello cards

**Feature:** manage todos in readme files 
  In order to not do everything twice
  As a meteorite I want to have new todos from my codebase show up in the readme file automatically
  
**Feature:** mail reminder
  In order to never forget a todo
  As a meteorite I want to receive email reminders on todos
