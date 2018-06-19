# nyt-react-search
New York Times article search and save with Mongo, Express, React, &amp; Node


## Props
Props are arbitrary, immutable inputs that are used to support components get rendered correctly to the DOM. Like attributes in HTML, they can hold pertinent information about how the component/element should look, what order it goes in, it's unique identifier, or what content is displayed through it.

Since they are immutable, props allow the developer to be more strict about what type of data can be used in the components they are assigned to. For even stricter definitions of props, you can use PropTypes to set certain requirements for the different props being used.

## State
State is the main source of data in your app. It is typically a JavaScript object that holds all of the data that will be called upon, edited, and/or used in your app. Best practices call for state to be managed at the top level container component and passed down to child components so there isn't data being changed around all over the place in your app. 

State can be updated from multiple sources such as a database, user input, or an external API.

## Component Lifecycle
**componentWillMount** is executed before rendering on both server and client side.

**componentDidMount** is executed after the first render only on the client side. This is where AJAX requests and state updates will occur. This is done after the component mounts in case there is an error with the data/state being updated by these requests, that way the component doesn't break before mounting. 

**componentWillReceiveProps** is invoked as soon as the props in the component are updated before another render is called.

**shouldComponentUpdate** should return a boolean "true" or "false" value and determine if a component should be updated or not. By default, it is set to "true", so you don't need to explicitely call this lifecycle unless you are looking for it to return "false".

**componentWillUpdate** is called just before rendering.

**componentDidUpdate** is called just after rendering.

**componentWillUnmount** is called after the component is unmounted from the DOM.