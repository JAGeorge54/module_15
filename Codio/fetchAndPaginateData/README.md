1. Fetch Data
React – Get Data
As you’ve seen in the course video, React allows you to fetch data from a remote source using useEffect and display it in a list on the web page. You can also add pagination to display the results in multiple pages.
Now, it’s time to practice getting data from the MIT Hacker News remote data source. In the first step of this activity you’ll add code that fetches the Hacker News data, as well as add new styles to the list of articles. Then, in the second step, you’ll add client-side pagination to display data on multiple pages.
The starter code for this activity is provided in the fetchData.jsx file.
In the first step of this activity, your task is to implement the fetchData method inside the useDataApi component, allowing it to get data from a remote source.
The fetchData async method dispatches the following actions:
FETCH_INIT: This is dispatched when fetchData is called
FETCH_SUCCESS: This is dispatched when the axios call is successful
FETCH_FAILURE: This is dispatched when the axios call has failed
Note: These actions can be found in the dataFetchReducer reducer.
Make use of the bootstrap list-group and list-group-item classes to style the list of articles returned by the data source. For reference, the formatting should match the following:
Note: This activity does not include the search feature shown in the course video and screenshot.
screenshot
Note: We are using useEffect so that our API call only runs when the component mounts (first render), and not also when the component re-renders.
Note: The didCancel boolean is for us to use in case of the component unmounts before the API call resolves (completes). We can prevent the state from being updated.