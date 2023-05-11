# 401 Advanced Python: Class 38 Reading Notes

## Summary: This class reading is about: React 3

What is React Context, and how does it help in managing state and data sharing in a React application?

  - React Context is a feature in React that allows you to share data between components without having to pass the data through props at every level of the component hierarchy.
  - It provides a way to pass data through the component tree without having to manually pass props down the hierarchy.
  - To use React Context, you first need to create a context object using the `createContext()` function.
  - Next, you need to create a provider component that will provide the data to the child components using the `MyContext.Provider` component.
  - The `value` prop is used to provide the data to the child components.
  - Any child component that wants to access this data can do so using the `useContext` hook.
  - React Context is useful for managing state and data sharing in a React application because it provides a way to share data between components without having to pass the data through props at every level of the component hierarchy.

Explain the useContext Hook and how it can be used to access data from a React Context within a functional component.

  - The `useContext` Hook is a feature in React that allows you to access data from a React Context within a functional component.
  - It is used to consume a context value that has been created using the `createContext()` function.
  - The `useContext` Hook takes the context object as an argument and returns the value provided by the nearest matching provider component.
  - The `useContext` Hook can only be used within a functional component or a custom Hook.
  - Using the `useContext` Hook to access data from a React Context within a functional component can simplify your code by eliminating the need to pass data through multiple levels of components via props.

    Another way of consuming context became available in React 16.8 with the arrival of React hooks. We can now consume context with the useContext hook.

    Instead of using render props, we can pass the entire context object to React.useContext() to consume context at the top of our component.

Here is the example above using the useContext hook:

```
    import React from 'react';

    export const UserContext = React.createContext();

    export default function App() {
      return (
        <UserContext.Provider value="Reed">
          <User />
        </UserContext.Provider>
      )
    }

    function User() {
      const value = React.useContext(UserContext);  
        
      return <h1>{value}</h1>;
}
```

Next.js is a React framework for building scalable web applications. The "E-Commerce Storefront" example demonstrates Next.js's scalability by utilizing server-side rendering, dynamic routes, data fetching, and serverless functions for an efficient e-commerce website.