---
layout: post
title:      "React Component Lifecycle"
date:       2021-07-04 03:17:27 +0000
permalink:  react_component_lifecycle
---


All components in React have their own lifecycles.  It begins when they are called to be rendered, lasts while they're displayed, and finishes when they are no longer being called.  React provides functions we use during each stage of the component lifecycle.  I am going to explain the component lifecycle through this blog post.  Note that some of the Component Lifecycle Hooks are used more than others, so they may not all be familiar and that's ok! 

1. Initializing - This occurs when the component is being set up and props and state are being passed and set up.
2. Mounting - This is when the component is actually rendered to the page and immediately after it's been rendered.
3. Updating - This stage is optional because it only kicks in when there is an update to a prop passed into the component or state within the component.
4. Unmounting - The last stage where the component is removed from the page.


In depth details about each stage:

## Initializing 

In this first stage, the component is being prepared to be ready.  The getDerivedStateFromProps( ) hook is used while the component is being initialized and before it's rendered to the page.  It takes "props" and "state" as parameters.  

## Mounting

The second stage is one that's used much more often than the first stage.  The two main lifecycle hooks that get called in this stage are: 
1.  render( ) 
2.  componentDidMount( )

Render actually is used during a few different lifecycle stages.  The first time it's called is when the component is first loaded onto the page.  Here is an example:

```
class App extends React.Component {
          render( ) {
					   return(
						    <div className="App">
								   <p>App</p>
							   </div>
						   )
					}
}					
						
```


One thing to keep in mind is that if we need to write Javascript inside of the render( ) function, it should be done BEFORE the return statement.

componentDidMount( ) gets called immediately after the render( ) method is called and the component is loaded to the page.  One common use for this hook is to make an API call to fetch data.  Another common time to use componentDidMount( ) is when we have Javascript that depends on content already being rendered on the page.


## Updating

The update stage kicks off whenever a prop passed into a component changes, or an item in state within a component changes.  In this phase, we call the render( ) method again, along with a very common hook, componentDidMount( ).   There are also a few less-used hooks in this stage.  For example: getDerivedStateFromProps( ), shouldComponentUpdate( ), along others.

componentDidUpdate( ) gets called immediately after render( ) executes due to an update.  It receives three parameters automatically:
1. previous props
2. previous state
3. snapshot


## Unmounting

The final stage uses a single hook that gets called right before a component is removed from the DOM.  This helps clean up anything in memory, like event listeners added to non-React elements in the DOM.  For example, when an App component uses a timer and the timer runs out, it is usually removed from the page.  componentWillUnmount( ) could be used to stop the timer and log a message telling that the component is about to be removed.  This isn't used often, but can come in handy sometimes.


There is a lot to remember from the Component Lifecycle.  The good thing is there are only two main hooks used often, componentDidMount( ) and componentDidUpdate( ).  It is good to know about the other components, but as a beginner, I've learned it is alright to focus on the main ideas to start.  The rest will come into place eventually!









