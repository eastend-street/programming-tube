<h1>Codeo</h1>  

[![Netlify Status](https://api.netlify.com/api/v1/badges/a988417b-7170-4f7b-9ece-0bb06a035b38/deploy-status)](https://app.netlify.com/sites/keen-noyce-db7b77/deploys)

Codeo is a website where you can search for programming videos from Youtube📺

website: https://codeo.netlify.app/

<br/>

<a href="https://codeo.netlify.app/" target="_blank">![Screen Shot 2019-12-18 at 8 15 53 PM](https://user-images.githubusercontent.com/43656115/71144579-5bc9f680-21d3-11ea-9b65-98c6fb660d17.png)</a>


<br/>

## Why I created this app
To search programming video easily. Youtube has a lot of programming youtube but there is not category page for programming. That's why I made Codeo.

<br/>

## Technologies
- React.js
- React hooks
- React Context API
- Redux
- TypeScript
- JavaScript
- YouTube Data API

<br/>

## User Interface
![codeo-ui](https://user-images.githubusercontent.com/43656115/76177731-6791dd00-6172-11ea-928d-6ceb16a43e5f.png)


<br/>

## Architecture
![codeo-architecture](https://user-images.githubusercontent.com/43656115/76172534-54701480-6154-11ea-8dd3-09b45f41d475.png)

<br/>

## State management
On this project, I adopted a **hybrid of React hooks and Redux**. Because it's going to be easier to manage state.  
I use Context API to provide state to child components at a lower level. Also, state is managed by Redux but I don't have to use `mapStateToProps` or `mapDispatchToProps`. Instead of those, using React hooks such as `useContext`. On the App component, I defined `state` and `dispatch`, they are provided to child components using Context API. Then on a child component, getting state using `useContext`.

![app.tsx](https://user-images.githubusercontent.com/43656115/76173223-bfbce500-615a-11ea-9849-0c9774a3f8d5.png)

<br/>

## Structure
```
src/
 index.tsx
 
 actions/  -----Actions to call API and dipatch data to Redux 
   EACH-CATEGORY.ts/
 
 components/
   COMPONENT_NAME/
    |-- COMPONENT_NAME.tsx  -----components with styled-components
 
 contexts/ ----- Create React context API
 
 reducers/  -----Get data from actions to send it to store 
   EACH-CATEGORY.ts/
 
 assets/
  images/ 

 data/  ----- Youtube video json data for failing to call API
 
 utils/ ----- common functions
```
<br/>


## Upcoming features
- Put mask on other movies, when a movie is selected
- Make sort function by date, views, upvote

<br/>

## Author
[eastend-street](https://github.com/eastend-street)

