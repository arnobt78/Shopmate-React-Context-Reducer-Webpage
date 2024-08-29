
## Shopmate-React-Context-Reducers-Webpage

Shopmate is a demo React E-Commerce Web Application (Global Level State Application), using React "useContext" and "useReducer" features. React Core, Hooks, Routing, HTML, CSS, Responsive Screen, Context, and Reducers functionalities have been used in this project and deployed on Netlify.

**Note:** "useContext" and "useReducer" have been employed in this React project; "Redux" and "Redux-Toolkit" have not been used here.

**This webpage can be seen by using this URL:** 

## To Install Dependences

Before launching this web application, be sure to install all required dependencies, which are listed in the package.json file.

To install all dependences, run this command from your project folder: `npm install`

## To Install NodeJS

Make sure you have NodeJS installed in your machine first, The installation instructions are here: https://nodejs.org/en/

## To Install React-Router 

Open up your terminal and bootstrap a new React app by: `npx create-react-app`

Then go to that project folder, and write this command via terminal from your project folder: `npm install react-router-dom`

(To check for more details about React-Router, please visit: https://reactrouter.com/en/main )

## About React Context and Reducers

- **useContext**: Global State Management

Used to save state globally so the state is available globally in our application.

- **useReducers**: Perform Actions On Global State

Allow us to manage complex state logic.

Vocab,

- `context` - an API given to us by React, allowing for the passing of information to child components without the use of props
  
- `reducer` - a pure function, accepting a state & action, and returning a new state
  
- `action` - an object literal, which describes a change to the state
  
- `useContext` - a react hook, that allows functional components to take advantage of the context API
  
- `useReducer` - a react hook, used in place of `useState`, generally for more complex state
  
- `dispatch` - a function returned to us by `useReducer`, which sends action objects to the reducer function

**context/CartContext.js**

1. Create a ‘context’ folder with ‘CartContext.js’ file inside it

2. Define initialState

3. Create CartContext using createContext with initialState

**context/cartReducer.js**

1. Create a ‘reducer’ folder with ‘cartReducer.js’ inside it

2. Create cartReducer function with parameters as state and action

3. Define all operations as switch statements inside the cartReducer

**context/CartContext.js**

1. Create CartProvider accessing the children

2. Access state and dispatch using useReducer with cartReducer and initialState

3. Define function for each possible operation

4. Use dispatch to execute the operation along with type and payload

5. Return the CartContext.Provider with children and prop value
Values that you want to access inside the entire application

6. Create useCart function, 
- Define context using useContext(CartContext)
- Return the context

**App.js**

1. Wrap entire App with CartProvider

**CartCard.js**

1. Access all values using useCart()

2. Add a condition to restrict ‘Add To Cart’ for one-time use for each product 

**Cart.js**

1. Access cart items and total using useCart()

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
