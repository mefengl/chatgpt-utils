# chatgpt-utils

getSubmitButton, getTextarea, getRegenerateButton, getNewChatButton...

```js
const getSubmitButton = () => {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  const result = buttons[buttons.length - 1]; // can also use: const result = Array.from(buttons).find(button => button.textContent.trim().toLowerCase() === 'submit');
  return result;
};
```

```js
const getTextarea = () => {
  const form = document.querySelector('form');
  const textareas = form.querySelectorAll('textarea');
  const result = textareas[0];
  return result;
};
```

```js
const getRegenerateButton = () => {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  const result = Array.from(buttons).find(button => button.textContent.trim().toLowerCase().includes('regenerate')); // can also use a for loop
  return result;
};
```
