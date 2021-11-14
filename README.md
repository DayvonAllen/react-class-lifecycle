## React App Lifecycle(Class Based Component)
1. JS file is loaded by the browser.
2. Instance of App Component is created.
3. App Component's 'constructor' function gets called.
4. State object is created and assigned to the 'this.state' property.
5. React will execute all logic above the `render` method.
6. React calls the component's `render` method.
---

## Component Lifecyle Steps(CLass Based Component)
1. `constructor`
   - Good place to do one-time setup.
2. `render`(required, called everytime an update is made)
   - Avoid doing anything besides returning JSX.
3. `componentDidMount`(at this point content is on the screen, called one time only; can optionally execute code in this method)
   - Good place to do data-loading. 
4. `componentDidUpdate`(sit and wait for updates, called everytime an update is made;  can optionally execute code in this method)
   - Good place to do more data-loading when state/props change. 
5. `componentWillUnmount`(sit and wait until this component is no longer shown, called one time only;  can optionally execute code in this method)
   - Good place to do clean up(especially for non-React stuff).
---

## All Lifecycle Methods
- `componentDidMount`
- `componentDidUpdate`
- `componentWillUnmount`
- `shouldComponentUpdate`(Rarely used)
- `getDerivedStateFromProps`(Rarely used)
- `getSnapshotBeforeUpdate`(Rarely used)
---