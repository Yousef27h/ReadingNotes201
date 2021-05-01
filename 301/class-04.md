# Forms

1. What is a ‘Controlled Component’?

 A __controlled component__ is an input form element, which value is being controlled by React state be the "single source of truth"

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We should update the state responses as soon as the user inputs a response, because we want our UI elements to be reponsive to the user response as soon as they change it to give it more dynamic feeling.

3. How do we target what the user is entering if we have an event handler on an input field?

we target the user input by using `event.target` inside the form's event handler.

# Conditional (Ternary) Operator

1. Why would we use a ternary operator?

To execute the same lines of codes in fewer lines, which makes the code more efficient and looks more professional 

2. Rewrite the following statement using a ternary statement:

```
if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

```
x===y ? console.log(true) : console.log(false);
```


## Things I want to know more about

I want to know the correct answers for questions in "Forms" reading.

# Forms 

There are few differences between a straight HTML form and a JavaScript-enhanced form. The main one being that a JavaScript form relies on one or more event handlers, such as onClick or onSubmit. These invoke a JavaScript action when the user does something in the form, like clicking a button.

In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.


We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

