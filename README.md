# <h2>React Interview Questions</h2>

**React Fiber vs Reconciliation:**

🚀Reconciliation is an algorithm that React.js uses to differentiate one tree from another to determine which parts need to be changed. Basically, it keeps track of UI and data layers when there is diff in both layers react using virtual DOM and updates the changes by re-rendering the specific component.

🚀React Fiber is used to increase React's suitability for areas like animation, layout, and gestures. Its headline feature is incremental rendering: the ability to split rendering work into chunks and spread it out over multiple frames.
Basically, react fiber is an architecture that splits the work and updates the only component that needs to change.


**React Components styling**

React Components can add styling in the following ways:

<ul><li>Add the Global Styles to the “index.html” File</li>
<li>Create a Style for Each Individual Component</li>
<li>Adding Inline Style to React Component Elements</li>
<li>Attach style property to JavaScript Style Object</li></ul>


**Different Ways to Fetch Data in ReactJS**

<ul>
  <li>Fetch method</li>
<li>Async-Await</li>
<li>Axios library</li>
<li>Custom Hook</li>
  <li>React Query Library</li>
</ul>

**What are pure functions in react?**

A pure function is a function that consistently produces the same output for a given set of inputs and doesn't have any side effects, such as modifying external state or performing actions beyond computing the output which brings some advantages like 👇

<ul>
<li>Predictable output</li>
<li>Easy to reason about and refactor code</li>
<li>Easy to test</li>
<li>Helping in performance optimization</li>
  </ul>

**Keys in reactjs**

A key is a unique identifier and it is used to identify which items have changed, are added, or are removed.

Why we shouldn't use an index as a key to the React component.

<ul>
<li> When components are using an index as a key, React distinguishes between them based on their key.</li>
<li> Let's say, we delete the first element at the index 0 position, the other elements will be re-indexed from 0,1,2,3.</li>
<li>In this case, Each component has a different index as compared to the last render.</li>
<li>React thinks that these all are new updated components, hence it will render all those comments.</li>
  <li>So you got the idea that it is not efficient for performance.</li>
</ul>

**React Performance Optimization Tips**

<ul>
<li>Use React Fragment to decrease the usage of extra HTML wrappers</li>
<li>Apply the lazy Loading concept</li>
  <li>Memoizing react component using React.memo()</li>
  <li>Avoid inline functions in render function</li>
  <li>Avoid using the index as a key</li>
  <li>use useCallback hook</li>
  <li>Production Mode Flag in webpack</li>
</ul>

**React Hooks**

**useState:** Manage your component's state with ease. Get the current state and a function to update it.

**useEffect:** Master side effects like data fetching and DOM manipulation. It runs after rendering, ensuring seamless interaction.

**useContext:** Simplify context data access, eliminating prop drilling and keeping your code clean.

**useReducer**: Tackle complex state logic effortlessly. Think of it as a supercharged useState.

**useCallback:** Supercharge your functions. Optimize performance by memorizing functions and controlling their re-creation.

**useMemo:** Optimize expensive computations. Calculate results only when dependencies change.

**useRef**: Unleash DOM magic. Create a ref object for persistent values without re-renders.


**Higher order component**

A higher-order component is a function that takes a component as an argument and returns a new component that wraps the original component.
They allow you to reuse component logic across multiple components.

Example: Authentication, Logging, Styling and Theming

**Child props**

In React, the props.children property refers to the child elements that are passed to a React component.

For example, in the following code:

`<MyComponent>`

 ` <div>Child 1</div>`
 
  `<div>Child 2</div>`
  
`</MyComponent>`

**How to handle errors in reactjs?**

<ul>
<li>Try and Catch</li>
<li>React Error Boundaries</li>
</ul>

**How to pass data from a child component to its parent in ReactJS?**

In the parent component, create a callback function. This callback function will retrieve the data from the child component.

Pass the callback function to the child as a props from the parent component.

The child component calls the parent callback function using props and passes the data to the parent component.

**Why functional components are better than Class components?**

In a class component, there are three steps to compile the JavaScript: First, you transform the class into a function, then you render it. However, in a functional component, there are only two steps: function definition and rendering. This eliminates the need for transforming a class into a function.

**Prop drilling**

Prop drilling occurs when a parent component passes data down to its children and then those children pass the same data down to their own children.


Prop drilling can become a significant pain point as your React application grows in complexity. By using the Context API and Hooks, you can avoid prop drilling and create a more maintainable and flexible application. With these tools, you can efficiently manage the state and ensure a cleaner, more readable codebase.

**Why you can't update props in React?**

The React philosophy is that props should be immutable and top-down. This means that a parent can send any prop values to a child, but the child can't modify the received props.

**Destructuring in React**

In the JavaScript and React world, object and array destructuring are powerful features that allow developers to extract data from arrays or objects into distinct variables. This is particularly useful when dealing with complex state objects or props in a React component.

>const vehicles = ['mustang', 'f-150', 'expedition'];

>const [car, truck, suv] = vehicles;

**How to iterate objects in react**

<ul>
<li>To loop through an object in React:

Use the Object.keys() method to get an array of the object's keys.
</li>
<li>
If you need to loop through an object's values:

Use the Object.values() method to get an array of the object's values.</li>
<li>
Loop through an Object's entries in React
>
You can also use the Object.entries method which returns an array of key-value pair arrays.</li></ul>

<img width="647" alt="image" src="https://github.com/Sathyaraj-dev/reactjs-interview-preparation/assets/57762726/c9a2ed2a-ea71-4131-9f71-83415e0d14ad">


**What is the significance of the render() method in React.js?**

The render() method in React.js is responsible for returning the JSX that represents the structure and appearance of a component. It gets called whenever the
component updates.

**ReactJS Error: An identifier or keyword cannot immediately follow a numeric literal**

For this response {reponseData?.5g_features.section_heading}

The property 5g_features starts with a digit, which causes the issue. To access a property that starts with a digit, you need to use bracket notation.
{reponseData?.['5g_features'].section_heading}

**When should you use useState vs. useReducer in React?**

Use `useState` for simple state logic and `useReducer` for complex state logic that involves multiple sub-values or when the next state depends on the previous one.
