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
    - Whenever a property is changed, the render() method runs on the template.
    ```javascript
        npm install --save @vaadin/vaadin-text-field @vaadin/vaadin-button @vaadin/vaadin-checkbox @vaadin/vaadin-radio-button
    ```
    - Always create a new array. This guarentees render().

3. State management with Redux
4. Navigation and code splitting
5. PWA and offline