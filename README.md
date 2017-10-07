
# @ngrx/store

@ngrx/store is a set of Angular libraries for reactive extensions

@ngrx/store is a controlled state container designed to help write performant, consistent applications
on top of Angular. 

 #### What Is Reactive Programming?
  - Reactive programming is a way applications handle events and data flow in your applications. In reactive programming, you design your components and other pieces of your software in order to react to those changes instead of asking for changes. This can be a great shift.
  - Reactive programming is a shift in the way you communicate between different parts of an application. Instead of pushing data directly to the component or service that needed it, in reactive programming, it is the component or service that reacts to data changes.

#### Core Concepts
 - ngrx/store brings a Redux-like single store for all of your app state to Angular.

#### Store

The store can be seen as your client side database but, more importantly, it reflects the state of your application. You can see it as the single source of truth.

It is the only thing you alter when you follow the Redux pattern and you modify by dispatching actions to it.

#### Reducer
 
Reducers are the functions that know what to do with a given action and the previous state of your app.

The reducers will take the previous state from your store and apply a pure function to it. Pure means that the function always returns the same value for the same input and that it has no side effects. From the result of that pure function, you will have a new state that will be put in your store.

#### Actions

Actions are the payload that contains needed information to alter your store. Basically, an action has a type and a payload that your reducer function will take to alter the state.

#### Dispatcher

Dispatchers are simply an entry point for you to dispatch your action. In Ngrx, there is a dispatch method directly on the store.

#### Middleware

Middleware are some functions that will intercept each action that is being dispatched in order to create side effects, even though you will not use them in this article. They are implemented in the Ngrx/Effect library, and there is a big chance that you will need them while building real-world applications.
 

### Included
 - [@ngrx/store](https://github.com/ngrx/store) - RxJS powered state management for Angular apps, inspired by Redux
 - [@ngrx/effects](https://github.com/ngrx/effects) - Side effect model for @ngrx/store
 - [@angular/router](https://github.com/angular/angular) - Angular Router
 - [@ngrx/db](https://github.com/ngrx/db) - RxJS powered IndexedDB for Angular apps
 - [@ngrx/store-devtools](https://github.com/ngrx/store-devtools) - Instrumentation for @ngrx/store enabling time-travel debugging
 - [jest](https://facebook.github.io/jest/) - JavaScript test runner with easy setup, isolated browser testing and snapshot testing
 
 
## Why Use Ngrx? 

#### Complexity

The store and unidirectional data flow greatly reduce coupling between parts of your application. This reduced coupling reduces the complexity of your application, since each part only cares about specific states.
 
#### Tooling 
 The entire state of your application is stored in one place, so it is easy to have a global view of your application state and helps during development. Also, with Redux comes a lot of nice dev tools that take advantage of the store and can help to reproduce a certain state of the application or make time travel, for example.

#### Architectural simplicity
Many of the benefits of Ngrx are achievable with other solutions; after all, Redux is an architectural pattern. 

#### Small learning curve

Since this pattern is so widely adopted and simple, it is really easy for new people in your team to catch up quickly on what you did.

Ngrx shines the most when you have a lot of external actors that can modify your application, such as a monitoring dashboard. In those cases, it is hard to manage all the incoming data that are pushed to your application, and state management becomes hard. That is why you want to simplify it with an immutable state, and this is one thing that the Ngrx store provides us with.


## Building an Application with Ngrx

```bash
# Install the ngrx

   npm install ngrx --save
 

# Install the angular cli to cretae the angular projects:

   npm install -g @angular/cli
   
 # Create the project.
  
    ng new "Your project name"
    
```

 And Follow the [Building an Application with Ngrx](https://www.toptal.com/angular-js/ngrx-angular-reaction-application)

# Reference
[Building an Application with Ngrx](https://www.toptal.com/angular-js/ngrx-angular-reaction-application)
 




