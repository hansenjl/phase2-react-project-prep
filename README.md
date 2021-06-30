# Phase 2 React Project 

## Helpful Resources 
- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
- [JSON Server Collection](https://github.com/Dane-Dawson/json-server-collection)
- [Deploy your JSON server to heroku](https://github.com/jesperorb/json-server-heroku)
- [Raquel's Blog on Deploying to Heroku](https://dev.to/raquii/my-first-javascript-project-became-a-lesson-in-deploying-a-rest-api-json-server-and-how-you-can-do-it-too-5gh7)
- [JSON server documentation](https://www.npmjs.com/package/json-server)
- [React Router Documentation](https://reactrouter.com/web/guides/quick-start)


## Getting Started 
1. `cd` into the folder where you would like your phase 2 project to live. Then type `npx create-react-app name-of-app` to make your React app. 

2. Once the command is done running, `cd` into the project folder. 

3. Go to github and create a new repository. Look at the steps labelled *…or push an existing repository from the command line*. Copy those steps and paste them into your terminal. The commands you will copy should look like this: 

```
git remote add origin git@github.com:hansenjl/phase2-react-project-prep.git
git branch -M main
git push -u origin main
```

Refresh the Github browser page to make sure it updated correctly.

4. Plan out your React app. You will need 3 routes so start by drawing out what the 3 different routes will look like. Then, break that drawing down into components. 

5. Create the components and routes you think you will need and hard-code in any data just so you can get the component structure and heirarchy down. 

6. Spend time thinking about what you will need to keep track of in state and which components will be need access to that state. Remember, if 2 sibling components need access to the same state, it must be stored in the parent component. 

7. Set up your db.json. First install json server using this command: `npm install -g json-server`. Then create a file called db.json and add data to it. The data should be added like this: 
```
{
    "objects": [
        {
            "id": 1,
            "name": "Someone",
            "age": 10
        },
        {
            "id": 2,
            "name": "Another Person",
            "age": 100
        }
    ]
}
```

The file will always be structured like an object with keys pointing to an array of objects. In the above example, this would give you a route ending with '/objects'. To run the server on a specific port, use this command: `json-server --watch db.json --port 3004`

8. Check in the browser that you can see the data from your json server. 

9. Now you are ready to fetch your data from your react app and replace any "hard-coded" data. 

10. Once you have your data displaying, implement the fetch request for a POST or PATCH request to your json server. 