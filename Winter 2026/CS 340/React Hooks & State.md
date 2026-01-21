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
- dependency array is the same as useEffect
- often used with useMemo
## useMemo
- memoizes a value 
- returns a value usually an object

```ts
const toastActions = useMemo(
	() => {{
		displayExistingToast,
		displayToast,
		deleteToast,
		deleteAllToasts,
	}},
	[displayExistinToast, displayToast, deleteToast, deleteAllToasts]
)
```

## Common Built-in React Router Hooks
- useNavigate: Navigate to a route
```ts
import {useNavigate} from "react-router-dom";

const navigate = useNavigate();
navigate("/login);
```

- useLocation: access URL of current route
```ts
import { useLocation } from "react-router-dom";

const location = useLocation();
location.pathname.startsWith("/feed/)
```

 - useParams: Access URL path parameters of current route
 - useSearchParams: Access URL query parameters of current route

## Creating Hooks
create a type or interface definition of object that has the functions that will be returned
hooks are functions that start with the word use and returns functions

# States
## useState
- use within components to cause a rerender when the state value changes
- state variables are not re-initialized like a regular variable would be
- returns an array
	- element 0 is the state variable
	- element 1 is an update function that can be called to change the state value and cause the component to rerender
### Updater Functions
2 forms
1. setX(123)
2. setX(previous => 123)
```ts
setUserInfo((previous) => {
	return { ...previous, displayedUser: user}
});
```