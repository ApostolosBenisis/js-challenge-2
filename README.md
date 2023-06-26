# ReactJS Challenge

Stack
- ReactJS
- Fetch API
- [Notistack](https://notistack.com/getting-started)
- Jest and [React Testing Library for testing](https://testing-library.com/docs/react-testing-library/intro/) 

Topics:
- Component creation
- Asynchronous operations
- State management
- Error handling
- UI notifications
- Unit testing

## Introduction
In React applications, we often manage asynchronous operations like API calls. These need to be handled correctly, along with the application state and user notifications for a smooth user experience.

For this challenge, your task is to build a React component. On a button click, it should trigger multiple GET requests. For user notifications - successful or unsuccessful operations - we'll use [Notistack](https://notistack.com/getting-started).

## Challenge

### Level 1
Start by creating a React component that has a button. Clicking this button should initiate several GET requests. You can use the [JSONPlaceholder](https://jsonplaceholder.typicode.com/) API to simulate this. For example:
- https://jsonplaceholder.typicode.com/posts
- https://jsonplaceholder.typicode.com/comments
- https://jsonplaceholder.typicode.com/todos
- https://jsonplaceholder.typicode.com/users

### Level 2
Make sure to handle any errors during the GET requests. 

What kind of errors can you expect?

Consider edge cases, such as some requests being slow while others are quick, some succeeding while others fail. 

What would be your approach if you had to manage 100 such requests?

### Level 3
Once all the GET requests have been completed, display a simple notification text to the user.

- If all the requests have been successful, display a success notification.
- If any of the requests fail, an error notification should be displayed.

Use some element in the UI e.g. a `<p></p>` tag to display the notification text.

In the next step you will use [Notistack](https://notistack.com/getting-started) to display better notifications, so for now, just displaying the notification text is enough.

### Level 4
Once all the GET requests have been completed, use [Notistack](https://notistack.com/getting-started) to display a notification.

If all the requests have been successful, display a success notification. If any of the requests fail, an error notification should be displayed.

### Level 5
It's time to test your component. Using Jest and React Testing Library, make sure your tests cover the following scenarios:
- The component renders correctly.
- Clicking the button triggers the GET requests.
- The component handles errors properly.
- The success notification displays when all GET requests complete successfully.
- The error notification shows up when any GET request fails.

### Level 6
For an added touch, set a transition duration of 5 seconds for the notification snackbar ([Notistack SnackbarProvider Props](https://notistack.com/api-reference#snackbarprovider-props)). This means that the notification will appear gradually over 5 seconds.

How does this animation affect your tests? How can you accommodate for this in your testing process?