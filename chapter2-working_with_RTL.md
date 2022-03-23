# Working with React Testing Library

## Structuring tests with React Testing Library

- To structure and write our test code, we will use the Arrange-Act-Assert pattern that's
  typical in writing unit tests.
- The DOM Testing Library team recommends using the getByRole
  method to select elements as much as possible in the documentation.

## Testing presentational components

- Presentational components are
  components that do not manage state. Typically, you use presentational components to
  display data passed down from parent components as props or to display hardcoded data
  directly in the component itself.

- snapshots can be used to test the rendered html from the component. Good for when everything is hard coded.

## Using the debug method

- The debug method, accessible from the screen object, is a helpful tool in React Testing
  Library's API that allows you to see the current HTML output of components as you build
  out your tests.

```
it('displays the header and paragraph text', () => {
 render(<Travel />)
 screen.debug()
})
```

- You can use the debug method to log specific elements of the resulting component DOM
  to the screen:

```
it('displays the header and paragraph text', () => {
 render(<Travel />)
 const header = screen.getByRole('heading', { name:
 /travel anywhere/i })
 screen.debug(header)
})
```
