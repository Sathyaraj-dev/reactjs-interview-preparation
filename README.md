# <h2>React Interview Questions</h2>

**React Fiber vs Reconciliation:**

🚀Reconciliation is algorithm which React.js uses to differentiate one tree with another to determine which parts need to be changed. Basically it keeps the track of UI and data layers when there is diff in both layers react uses virtual DOM and updates the changes by re-rendering the specific component.

🚀React Fiber is used to increase React's suitability for areas like animation, layout, and gestures. Its headline feature is incremental rendering: the ability to split rendering work into chunks and spread it out over multiple frames.
Basically react fiber is a architecture which splits the work and updates the only component that needs to change.
