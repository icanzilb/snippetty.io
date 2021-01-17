# React ToDo App

## Intro

[React ToDo Starter](http://snippette.com/downloads/ReactToDo.zip)

Explain about the `App` component and its `render()` method. Mention the `ReactDOM.render(...)` call at the bottom of **index.js**.

Briefly show **index.css** to make parallel to "normal" web pages.

## Adding items to the list

Create a state property in App's `constructor()`:

```javascript
this.state = {items: []}
```

Add a button click event handler inside the `<button>` tag:

```javascript
onClick={this.add}
```

Add a class method to add new todo items:

```javascript
add() {
  const field = document.querySelector('.newItem')
  const value = field.value
  field.value = ''
}
```

Append to the new `add()` method:

```javascript
this.setState((state) => {
  return {items: state.items.concat([value])}
})
```

Do mention about using `this.setState()` vs. mutating `this.state`.

In `constructor()` bind the new `add()` method:

```javascript
this.add = this.add.bind(this)
```

Explain about how `this` works in JS and best practice of binding class methods in the constructor for later use.

## Sub-components

Introduce component props and briefly talk about state vs properties.

Add a new component to render list items:

```javascript
class Item extends React.Component {
  render() {
    return (
      <li key="{this.props.key}">{this.props.title}</li>
    );
  }
}
```

Insert inside the `<ol>` tag to render the todo list:

```javascript
{this.state.items.map((item, index) =>
  <Item key={index} title={item}/>
)}
```

## Finishing touches

Add "empty" message inside `<ol>` tag:

```javascript
{this.state.items.length === 0 &&
  <span>empty</span>
}
```

## Outro

Demonstrate the finished app and invite everyone to check the tutorials at reactjs.org