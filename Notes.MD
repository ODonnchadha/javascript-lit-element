- <https://vaadin.com/learn/tutorials/lit-element/starting-a-lit-element-project>

1. Starting a LitElement project
    - Getting started:
    ```javascript
        npm install
        npm run dev
    ```
    - Install dependencies:
    ```javascript
        npm install --save @polymer/lit-element
    ```
    - Implement the component itself.
    - And then complete the component registration.

2. lit-html templating and events:
    - Whenever a property is changed, the render() method runs on the template!
    ```javascript
        npm install --save @vaadin/vaadin-text-field @vaadin/vaadin-button @vaadin/vaadin-checkbox @vaadin/vaadin-radio-button
    ```
    - Always create a new array. This guarentees render().

    - By default, the content of a LitElement component is shielded from external CSS by a Shadow DOM. 
    - This is a feature that is valuable when building reusable leaf-node components. 
    - When building an application, it is often best to not create a shadow root to allow application-level styling.
    ```javascript
        createRenderRoot() {
            return this;
        }
    ```

3. State management with Redux
    - View -> Action Creators -> Reducer -> State -> View.
    - reselect: Middleware that lets us create optimized selectors for data that are derived from the state.
    - pwa-helpers: A collection of helpers for PWA that includes helpers for lazily connecting Web Components to a Redux store.
    ```javascript
        npm install --save redux reselect pwa-helpers nanoid
        npm audit fix
    ```
    - Redux DevTools extension: <https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en>
    - Every time the app state changes *stateChanged* gets called on the component and we can update the properties on our component.

4. Navigation and code splitting
5. PWA and offline