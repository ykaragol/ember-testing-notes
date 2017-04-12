# Testing Components

What to be tested in a component? A component consists of a behaviour and a template. A component serves a view with data, handles the user interactions and keeps internal states. When you want to test a component, you need to answer the question “what to be tested?”.

If you only want to test a computed property on a component, then the unit test fits for it. But if you want to test a component as a whole, then the integration test will be needed. By default an integration test is created when you create a component with ember-cli. This is because mostly components are tested with their templates, they have specific hooks those should be handled properly, also they use context such as injections.
During an integration test of a component, the following steps are used:
1. all component parameters and dependencies are created (or mocked)
2. component is rendered
3. interactions with the component are realized.

For those above steps, Ember Guide's “[Testing Components](https://guides.emberjs.com/v2.12.0/testing/testing-components/)” section is quite enough.

For further detail about mocking refer to the "[Mocking In Detail](./mocking-in-detail.md)" section of this notes.

For further detail about interaction with component refer to the "[Testing with UI Interactions](./testing-with-ui-interactions.md)" section of this notes.
