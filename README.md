# chatgpt-utils

getSubmitButton, getTextarea, getRegenerateButton, getNewChatButton...

```js
function getSubmitButton() {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  const result = buttons[buttons.length - 1];
  return result;
};
```

```js
function getTextarea() {
  const form = document.querySelector('form');
  const textareas = form.querySelectorAll('textarea');
  const result = textareas[0];
  return result;
};
```

```js
function getRegenerateButton() {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  const result = Array.from(buttons).find(button => button.textContent.trim().toLowerCase().includes('regenerate'));
  return result;
};
```

```js
function getNewChatButton() {
  const aElements = document.getElementsByTagName('a');
  const result = Array.from(aElements).find(a => a.textContent === 'New chat');
  return result;
};
```
