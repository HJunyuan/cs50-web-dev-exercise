# ⚙️ Part 3: JS

Make the web page interactive with JS (JavaScript) - not to be confused with Java.

**Link to exercise**: <a href="https://codepen.io/hjunyuan/pen/bGKKLWY" target="_blank">https://codepen.io/hjunyuan/pen/bGKKLWY</a>

## Step 1

Get the item value:

```javascript
const itemValue = document.getElementById("input_todo").value;
```

> This code segment gets the HTML element (where id is `input_todo`) and extracts its `value` property.
>
> As such, the variable `itemValue` now contains the text that the user has entered in the textbox.

## Step 2

Create a new `li` element with item value:

```javascript
const li = document.createElement("li");
li.textContent = itemValue;
```

> The first line of this code segment creates a new `li` element programmatically, which looks something like this:
>
> ```html
> <li></li>
> ```
>
> The second line of this code segment sets the text content to `itemValue` (obtained in the earlier step), which then looks something like this:
>
> ```html
> <li>Some text entered by user</li>
> ```

## Step 3

Add new item to list:

```javascript
const todoList = document.getElementById("list_todo");
todoList.append(li);
```

> The first line of this code segment gets the HTML element (where id is `list_todo`).
>
> The second line of appends the `li` element (created in the earlier step) to the `todoList`.
