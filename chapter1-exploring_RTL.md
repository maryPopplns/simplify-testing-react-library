# Exploring React Testing Library

## Introducing the DOM Testing Library

- The DOM Testing Library makes it easier to test the UI of applications like real users to gain confidence that the application works as expected for users. There are no methods to get the component's state value or directly invoke component methods. The library encourages you to select DOM elements in ways that are available to all users. The library's API includes accessibility-focused query methods allowing you to interact with the DOM like users with disabilities who require tools such as screen readers or other forms of assistive technology to navigate applications.

## Executing test cases with jest

- At a high level, Jest provides the describe,
  it, test, and expect functions to organize and execute tests. You can think of the describe function as a test suite. Use the describe function to group related tests for specific components. The it and test functions are for specific tests. The it and test functions are interchangeable functions used to house and run the code for individual test cases. Use the expect function to assert the expected output.

## Enhancing jest assertions with jest-dom

- Jest-dom provides two significant enhancements for Jest assertions. First, jest-dom provides over 20 custom DOM matchers that create more descriptive test code. Second, jest-dom also provides better context-specific error messages.

## Testing implementation details

- In most scenarios, tests that focus on the user provide more confidence than tests that focus on implementation details.
