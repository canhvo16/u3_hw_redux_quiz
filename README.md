# Redux Quiz

<img src="https://chriscourses.com/img/blog/redux/redux.jpg" height="400px"/>

## Getting Started

- Fork and Clone

## Questions

1. What is Redux?

```
Redux is a library that helps us manage our State so we can use them from anywhere in our app rather than having to pass them down the tree as props.
```

2. What packages do we install to use Redux?

```
npm install react-redux redux
```

3. In your own words, describe the flow of how Redux is used to manage state.

```
First we set up our Store, which houses all of our states, and Provider, which gives us access to the Store. When an interaction is made on the UI, that event handler determines what type of actions happen to the payload. And the payload goes through the reducer which denotes the action and the state is altered accordingly.
```

4. What do we use in order to manage different pieces of state?

```
Reducers are used to break up our state into little modules that we can perform Actions on
```

5. What do we use to perform an update to state?

```
Actions are used to update state
```

6. How do we access state from Redux?

```
In the component you are trying to access the state, you must have a function like mapStateToProps which takes state as an argument and allows us to assign the pieces of state we need as values inside an object. From that object we use dot notation on props to use the values that we need.
```

7. In your own words, describe how to set up Redux for a React App.

```
First you have to make sure your index.js is set up properly for React v.18

You have to run npm install react-redux redux

Inside the src folder, you need to create a store folder which will hold folders for Actions, Types, and Reducers

Inside the store folder, you need to create an index.js where you'll import createStore from redux, have createStore stored in a variable, and ahve the variable exported

Import that variable along with Provider from react-redux in the root index.js file and wrap your App component with Provider with store passed in

Once your Types are set up and exported, import them into your Actions and apply them appropriately to the correcct Action. Make sure that you are exporting your Actions

In your Reducers, you will write out the logic that will be performed based on each Action Type.

In the component that will use states from the Store, you ahve to import connect from react-redux and have that exported passing the mapStateToProps, which gives us access to our props in an object, and mapActionsToProps, which allows us to assign Actions to our state, as props.
```

## Submission

Pull Request due by **9AM EST** following the [PR Submission Guidelines](https://github.com/SEI-R-2-22/template_pull_request).
