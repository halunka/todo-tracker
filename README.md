# todo-tracker
A meteor app that checks your codebase for TODO's 

## Elevator Pitch
For developers…</br>
…who want to keep track of the todos in their codebase…</br>
…Todo Tracker…</br>
…is a todo tracker…</br>
…that automagically creates trello cards for the todos in your codebase…</br>
…unlike other todo trackers…</br>
…it is open source and just works…</br>

## Feature Stories
**Feature:** list todos from github repos</br>
  In order to keep track of my todos</br>
  As a meteorite I want to see a list of my todos</br>

  **Scenario:** log in with github</br>
    **Given** I am not logged in</br>
    **When** I click on ‘log in with github'</br>
    **And** I fill in ‘username’ with my username</br>
    **And** I fill in ‘password with my password</br>
    **Then** I should see ‘Add repo’</br>

  **Scenario:** add repo</br>
    **Given** I am logged in</br>
    **When** I click on ‘Add repo’</br>
    **And** I fill in ‘Owner name’ with the owner name</br>
    **And** I fill in ‘Repo name’ with a repo name</br>
    **Then** I should see ‘Repo name’</br>

  **Scenario:** view repo</br>
    **Given** there is a repo</br>
    **When** I click on ‘Repo name’</br>
    **Then** I should see ’Todo 1’</br>

  **Scenario:** remove repo</br>
    **Given** there is a repo</br>
    **When** I click on ‘Delete repo’</br>
    **Then** I should see ‘You have not yet added any repos’</br>

**Feature:** cli</br>
  In order to work comfortably from within the terminal</br>
  As a meteorite I want to use a cli</br>

**Feature:** daily recap</br>
  In order to keep track of my todos at all times</br>
  As a meteorite I want to receive recaps via email on a daily basis</br>

**Feature:** trello integration</br>
  In order to work with the kanban technique</br>
  As a meteorite I want to see my todos as trello cards</br>

**Feature:** manage todos in readme files</br>
  In order to not do everything twice</br>
  As a meteorite I want to have new todos from my codebase show up in the readme file automatically</br>
  
**Feature:** mail reminder</br>
  In order to never forget a todo</br>
  As a meteorite I want to receive email reminders on todos</br>

