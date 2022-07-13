# Project 2 - Bob's Burger 🍔

A pair programming project. Building a React app that receives a third-party API.

## Project Overview

The React app had to built within 1,5 days (hackathon) and must display information taken from a third-party API.

We decided to create an app that serves as a Wikipedia for the Bob's Burger cartoon, using their API.

## Technologies/Languages Used

- HTML5
- CSS3
- SASS
- Bootstrap
- JavaScript ES6+
- React
- Axios
- Yarn
- NPM
- Git
- GitHub

<img width="1512" alt="Screen Shot 2022-06-30 at 12 25 59 AM" src="https://user-images.githubusercontent.com/103049873/176547726-eeefcc9d-3267-4411-975b-fbdb04b7184d.png">

## Planning

<img width="788" alt="175276237-b6ea2d98-552c-4e8e-a8e8-1f8e296ce61d" src="https://user-images.githubusercontent.com/103049873/178732235-c53e983b-0d9c-412e-9990-fca28d679456.png">

We began by discussing a quick plan. We knew we wanted to create something fun, and spent a little while trying to find a good free API to use. This proved to be fairly difficult. Once we settled on using the Bob's Burger API we decided on which features to include. We knew we wanted a live search bar.

## The Build

As we were using a third-party API, we used Axios to serve our front-end. 

In order to display all the information for each respective artist on the page, 'dot notation' is used. In addition, a `.map()` is used to iterate through each character in the list.

## Home Page

Character Index Once landing on the Character Index page, an async function will run. This code block has been sectioned with a try/catch statement and will await the promise from axios, then set the data in state. This then allows us to cherry pick or manipulate the data which we draw from the API, and in this instance we are requesting for the characters to be returned.

<img width="485" alt="175278046-bac132c2-c4fa-4333-adb6-185fb02eae4d" src="https://user-images.githubusercontent.com/103049873/178732713-6576b0ea-4293-4c16-ad8f-5502855b4eac.png">


## Search Feature

The search filter on each page was implementing using a combination of useState and useEffect, where when the value of the text input box changed, we would update the filters state, then use this to create a filtered array.

Within this handleChange() function below, while we could have achieved the same result with simiply `setFilters(e.target.value)`, we set the state as an object to keep the door open for additional filtering options in the future.

Once we defined the filter state, we filtered the array we fetched from the API uisng RegExp, allowing us to only display recipes that meet the search term.

<img width="855" alt="Screen Shot 2022-06-30 at 12 52 48 AM" src="https://user-images.githubusercontent.com/103049873/176551794-853b60b7-5d29-4cd6-b86a-34abf0d63f4c.png">


Users are simply able to type in their desired character and the page will display a profile picture, ocuppation, the voice over actor and their first apperance on the show. 

For further informations about the character the user can press the "Wiki" button which is going to take him to a dedicated web page just for that character. 

<img width="1512" alt="Screen Shot 2022-06-30 at 12 39 21 AM" src="https://user-images.githubusercontent.com/103049873/176549795-c5f54b09-b33f-4441-a3ff-09fd45229947.png">

<img width="1512" alt="Screen Shot 2022-06-30 at 12 27 29 AM" src="https://user-images.githubusercontent.com/103049873/176547949-1dd60496-725f-4d1c-9c76-fcf3f18e7be4.png">


## Wins

- Getting data successfully to display on our page with Axios was of course a huge win as this provides the core functionality of the app.
- I think implementing the user search bar with an `onChange={function}` was definitely a fun problem to solve.
- Getting the project done in under 36 hours. 

## Challenges

- Our main issue was finding a good free API. As that took us half a day we were behind the schedule with the planning and coding. 

## Key Learning Points

- Axios: As this was both our first project using Axios to receive data from an API, it was crucial to practice and get to know how to use it. We enjoyed working out how render information on the page with using this.
- Team Communication: Building on teamwork skills was definitely another key-learning point. It was great practice being able to communicate changes to code, what needed to be completed and just conversing with each other, talking through problems that had arisen during the build!


