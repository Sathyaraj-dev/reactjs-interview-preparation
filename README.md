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


