# React Hooks
- start with the word 'use' and returns a value, object or array
- can only be accessed from React functional components or other React hooks

1. useEffect
2. use Callback
3. useMemo
4. useState
5. useContext
6. useRef

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

## useCallback
- memoizes a function to avoid unnecessary recreations between renders
	- memoize = stores a function reference and returns the same function (instead of recreating it)
- returns a function
- avoids overuse
```ts
const displayExistingToast = useCallback((toast: Toast) => {
	setToastList((previousList) => [...previousList, toast]);
}, [])
```
- dependency array is the same