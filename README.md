# chatgpt-utils
getSendButton, getNewChatButton, getRegenerateButton...

```js
const get_submit_button = () => {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  const result = buttons[buttons.length - 1]; // by textContent maybe better
  return result;
};
```

```js
const get_textarea = () => {
  const form = document.querySelector('form');
  const textareas = form.querySelectorAll('textarea');
  const result = textareas[0];
  return result;
};
```

```js
const get_regenerate_button = () => {
  const form = document.querySelector('form');
  const buttons = form.querySelectorAll('button');
  for (let i = 0; i < buttons.length; i++) {
    const buttonText = buttons[i].textContent.trim().toLowerCase();
    if (buttonText.includes('regenerate')) {
      return buttons[i];
    }
  }
};
```
