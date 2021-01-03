# Elm Boilerplate for WebExtension

This repo contains a basic boilerplate to develop extensions for Firefox
and Google Chrome using Elm. It relies on `webextension-polyfill` to ensure cross-browser compatibility.

## Development

Run `npm-watch` to watch the elm directory for changes and compile the code.


Run `web-ext run` to start a Firefox instance with your extension installed.
Refer to the MDN documentation for further docs on `web-ext`.


## Files

```
src/
├── manifest.json
├── elm/
│   ├── Background.elm          : Elm app of the background script
│   ├── Popup.elm               : Elm app of the browser action
│
│
├── elm-background-loader.js    : load Elm code into background script
├── background.html             : entry point for the background script
├── popup/
│   ├── index.html              : entry point for the popup
│   ├── elm-popup-loader.js     : load Elm into the popup HTML
```

## FAQ

Q : How do I add a page action ?  
A : A page action should be pretty similar to the background script.
  
  
Q : Does this work with Elm version <X> ?  
A : Yes, just re-create the elm apps with whatever version you need.
