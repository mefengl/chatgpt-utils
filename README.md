# ChatGPT Utils

[![AI Friendly](https://img.shields.io/badge/AI-Friendly-pink?style=for-the-badge)](https://github.com/mefengl/made-by-ai)
[![AI Assisted Maybe](https://img.shields.io/badge/AI%20Assisted-Maybe-yellow?style=for-the-badge)](https://github.com/mefengl/made-by-ai)
[![Commit Messages by AI](https://img.shields.io/badge/Commit%20Messages%20by-AI-green?style=for-the-badge)](https://github.com/mefengl/made-by-ai)

## Notice

this repo will soon be put into `chat-kit`, you can find more about it in [chatgpt-playground](https://github.com/mefengl/chatgpt-playground)

## Description

getSubmitButton, getTextarea, getRegenerateButton, getNewChatButton...

## Usage

just copy and paste the code below

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
function getStopGeneratingButton() {
    const form = document.querySelector('form');
    const buttons = form.querySelectorAll('button');
    return Array.from(buttons).find(button => button.textContent.trim().toLowerCase().includes('stop generating'));
}
```

```js
function getNewChatButton() {
  const aElements = document.getElementsByTagName('a');
  const result = Array.from(aElements).find(a => a.textContent === 'New chat');
  return result;
};
```

## Contributing

Contributions, issues and feature requests are welcome!

## License

This project is licensed under the terms of the [MIT license](/LICENSE).
