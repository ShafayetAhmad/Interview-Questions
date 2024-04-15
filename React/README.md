# React Interview Questions

This document contains a list of React interview questions that are commonly asked during job interviews. You can use these questions to practice, or to test your knowledge before an interview.

## Table of Contents

1. [Introduction to React](#introduction-to-react)
2. [Components](#components)
3. [Props](#props)
4. [State](#state)
5. [Lifecycle Methods](#lifecycle-methods)
6. [Hooks](#hooks)
7. [Event Handling](#event-handling)
8. [Conditional Rendering](#conditional-rendering)
9. [Lists and Keys](#lists-and-keys)
10. [Forms](#forms)
11. [Context](#context)
12. [Error Handling](#error-handling)
13. [Code Splitting](#code-splitting)
14. [Performance Optimization](#performance-optimization)
15. [Testing](#testing)
16. [Styling](#styling)
17. [State Management](#state-management)
18. [Routing](#routing)
19. [Server Communication](#server-communication)
20. [Best Practices](#best-practices)
21. [Miscellaneous](#miscellaneous)

## Introduction to React

<details>
  <summary>What is React?</summary>
  React is a JavaScript library for building user interfaces, developed by Facebook.
</details>

<details>
  <summary>What are the key features of React?</summary>
  Key features of React include:
  - **Component-Based Architecture**: Building UIs using reusable components.
  - **Virtual DOM**: Efficiently updating and rendering UI elements.
  - **JSX**: JavaScript syntax extension for writing HTML within JavaScript code.
  - **Unidirectional Data Flow**: Data flows in one direction, simplifying state management.
</details>

<details>
  <summary>What is the difference between React and ReactDOM?</summary>
  React is the JavaScript library for building UI components, while ReactDOM is the package responsible for rendering these components in the DOM.
</details>

<details>
  <summary>What is the significance of the Virtual DOM in React?</summary>
  The Virtual DOM is a lightweight copy of the real DOM. React uses it to perform efficient updates to the actual DOM by comparing the current Virtual DOM with the previous one and only updating the parts that have changed.
</details>

<details>
  <summary>Explain the concept of JSX in React.</summary>
  JSX (JavaScript XML) is a syntax extension for JavaScript that allows you to write HTML-like code within your JavaScript files. It simplifies the process of creating React elements and makes code more readable.
</details>

## Components

<details>
  <summary>What are React components?</summary>
  React components are reusable, self-contained modules that represent a part of the UI. They can be either functional components or class components.
</details>

<details>
  <summary>What is the difference between functional components and class components?</summary>
  Functional components are JavaScript functions that take props as input and return React elements. Class components are JavaScript classes that extend React.Component and can maintain their own state.
</details>

<details>
  <summary>When should you use functional components over class components?</summary>
  Functional components are preferred for simpler components that do not need state or lifecycle methods. They are easier to read, write, and test compared to class components.
</details>

<details>
  <summary>What are Pure Components in React?</summary>
  Pure Components are class components that automatically implement shouldComponentUpdate with a shallow prop and state comparison. They prevent unnecessary re-renders by only updating when the props or state change.
</details>

<details>
  <summary>Explain the purpose of the React.Fragment component.</summary>
  React.Fragment is a built-in component that allows you to group multiple children without adding extra nodes to the DOM. It is useful when you need to return multiple elements from a component's render method.
</details>

## Props

<details>
  <summary>What are props in React?</summary>
  Props (short for properties) are read-only data that are passed from parent to child components. They allow you to customize a component's behavior and appearance.
</details>

<details>
  <summary>Can you modify props inside a component?</summary>
  No, props are immutable and cannot be modified inside a component. They are passed down from the parent component and should be treated as read-only.
</details>

<details>
  <summary>How do you pass props from a parent component to a child component?</summary>
  You can pass props to a child component by adding attributes to the child component's JSX element, like `<ChildComponent propName={propValue} />`.
</details>

<details>
  <summary>What is prop drilling in React?</summary>
  Prop drilling is the process of passing props from a parent component down to multiple levels of nested child components. It can lead to cluttered and hard-to-maintain code, so it's often solved using context or state management libraries.
</details>

<details>
  <summary>Explain the concept of defaultProps in React.</summary>
  defaultProps is a property that you can define on a component to provide default values for its props. If a prop is not provided when the component is used, it will fall back to the default value specified in defaultProps.
</details>

## State

<details>
  <summary>What is state in React?</summary>
  State is a JavaScript object that represents the data specific to a component. It determines a component's behavior and renders UI based on changes to its data.
</details>

<details>
  <summary>What is the difference between state and props?</summary>
  - State is internal and managed within a component, while props are passed from parent to child components.
  - State can be modified within a component, while props are read-only and cannot be modified inside a component.
</details>

<details>
  <summary>When should you use stateful components over stateless components?</summary>
  Stateful components (class components with state) should be used when you need to manage and update component-specific data. Stateless components (functional components without state) are suitable for simple UI components that don't require data management.
</details>

<details>
  <summary>How do you update state in React?</summary>
  You can update state in React by calling the setState method provided by the React.Component class. It accepts an object or a function that returns an object containing the updated state values.
</details>

<details>
  <summary>What is the purpose of the useState hook in React?</summary>
  The useState hook is a built-in React hook that allows functional components to add and use state. It returns a stateful value and a function to update it, similar to this.state and this.setState in class components.
</details>
