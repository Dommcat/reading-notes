# 401 Advanced Python: Class 38 Reading Notes

## Summary: This class reading is about: React 2

How does lifting state up in a React application help with managing data flow and what are the benefits of using this approach?

Lifting state up in a React application means moving the state from a child component to its parent component so that multiple child components can access and manipulate the same state data. This helps with managing data flow in several ways:

  1. Centralizing state management: By moving state data up to the parent component, the state becomes centralized and easier to manage. Instead of keeping track of state in multiple child components, the parent component can manage the state and pass down the necessary data to its children.

  2. Avoiding duplication of state: When state is scattered across multiple components, it can lead to duplication of state and inconsistencies in the data. By lifting state up, the state data is stored in a single location and avoids duplication.

  3. Improving data consistency: When multiple components rely on the same data, lifting state up can improve data consistency. By storing the state in a single location, all components access the same source of truth, ensuring that the data is consistent across the application.

  4. Facilitating data sharing: When data needs to be shared between different components, lifting state up can facilitate this process. The parent component can pass the necessary data down to its children, allowing them to access the same data and coordinate their behavior.

  Overall, lifting state up in a React application helps with managing data flow by centralizing state management, avoiding duplication of state, improving data consistency, and facilitating data sharing. This approach can make React applications more efficient and easier to maintain.


Conditional rendering in React refers to the ability to display or hide certain components based on specific conditions. It allows developers to render different components or UI elements depending on the state of the application.

Here's an example of how to implement conditional rendering in a React component:

    ```jsx
    import React from 'react';

    function ExampleComponent(props) {
      const isLoggedIn = props.isLoggedIn;
      
      if (isLoggedIn) {
        return <div>Welcome, user!</div>;
      } else {
        return <div>Please log in.</div>;
      }
    }
    ```

In this example, the `ExampleComponent` receives a `isLoggedIn` boolean prop. Depending on the value of this prop, the component will render a different message. If `isLoggedIn` is `true`, the component will render the message "Welcome, user!". Otherwise, it will render the message "Please log in."

Another example could be conditionally rendering a button based on a certain state:

    ```
    import React from 'react';

    function ExampleComponent() {
      const [showButton, setShowButton] = useState(false);
      
      const handleClick = () => {
        setShowButton(!showButton);
      }
      
      return (
        <div>
          <button onClick={handleClick}>Toggle button</button>
          {showButton && <button>Click me!</button>}
        </div>
      );
    }
    ```

In this example, the `ExampleComponent` renders two buttons. The second button is only displayed if `showButton` is `true`. The `handleClick` function toggles the value of `showButton` when the first button is clicked. If `showButton` is `false`, the second button will be hidden. If `showButton` is `true`, the second button will be displayed.

Overall, conditional rendering in React is a powerful feature that allows developers to create dynamic and flexible user interfaces.

Thinking in React" is an approach to developing React applications that involves breaking the UI into a component hierarchy, building a static version of the UI, identifying where the state should live, creating a data flow model, and adding interactivity. By following these principles, developers can create maintainable, modular, and scalable applications that are composed of smaller, reusable components, and provide a better user experience.


## Re/Sources:

https://legacy.reactjs.org/docs/conditional-rendering.html

https://heroicons.com/


## Things I want to know more about

React "These docs are old and won’t be updated. Go to react.dev for the new React docs."