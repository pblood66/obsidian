# React Hooks
- start with the word 'use' and returns a value, object or array
- can only be accessed from React functional components or other React hooks

useEffect
use Callback
useMemo
useState
useContext
useRef

## useEffect
- use when you want to execute logic after your components render or rerenders
```ts
useEffect(() => {
	loadMoreItems();
}, []);
```

- last parameter is an optional dependency array
	- missing = invoke on every render
	- empty `[]` = invoke only initial render
	- A comma separated list of variables = invoke on the initial render and whenever one of the variables changes (use with props, state variables, callback functions, global variables)
