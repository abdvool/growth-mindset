# React and Forms

## Forms
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:


```
<form>
  <label>
    Name:
    <input type="text" name="name" />
  </label>
  <input type="submit" value="Submit" />
</form>

```
-------

### Controlled Components
In HTML, form elements such as < input >, < textarea >, and < select > typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

For example, if we want to make the previous example log the name when it is submitted, we can write the form as a controlled component:

```
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}

```
---------------

### Controlled Input Null Value
Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.

The following code demonstrates this. (The input is locked at first but becomes editable after a short delay.)

```
ReactDOM.render(<input value="hi" />, mountNode);

setTimeout(function() {
  ReactDOM.render(<input value={null} />, mountNode);
}, 1000)
```
---------------

### Alternatives to Controlled Components
It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library. In these situations, you might want to check out uncontrolled components, an alternative technique for implementing input forms.

---------------

## The Conditional (Ternary) Operator Explained

Starting With the Basics — The if statement

Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.
Consider the following example:
We have a person object that consists of a name, age, and driver property.
```
let person = {
  name: 'tony',
  age: 20,
  driver: null
};
``` 

We want to test if the age of our person is greater than or equal to 16. If this is true, they’re old enough to drive and driver should say 'Yes'. If this is not true, driver should be set to 'No'.

We could use an if statement to accomplish this:


```
if (person.age >= 16) {
  person.driver = 'Yes';
} else {
  person.driver = 'No';
}
```


But what if I told you we could do the same exact thing in just one line of code? Well, here it is:

```
person.driver = person.age >=16 ? 'Yes' : 'No';

```
-----------
Here’s what you need to know:

1- The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.

2 - A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.

3- Finally a : colon. If your condition evaluates to false, any code after the colon is executed.


### Example — Driver Age
We’ll take a moment to revisit the initial example in this article:

```
let person = {
  name: 'tony',
  age: 20,
  driver: null
};
person.driver = person.age >=16 ? 'Yes' : 'No';

```
The most important thing to note is the order of operations. Lets add some parenthesis to help you visualize the order in which code is executing:
```
person.driver = ((person.age >=16) ? 'Yes' : 'No';)

```

--------------
### Rewrite the following statement using a ternary statement:

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
  ```


  ```
 cosnole.log = x===y ? 'true' : 'false'
 ```
