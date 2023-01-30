# ChatGPT Chrome Extension but now in firefox🤖 ✨

A Chrome extension that adds [ChatGPT](https://chat.openai.com) to every text box on the internet! Use it to write tweets, revise emails, fix coding bugs, or whatever else you need, all without leaving the site you're on. Includes a plugin system for greater control over ChatGPT behavior and ability to interact with 3rd party APIs.

![](https://i.imgur.com/CPMOyG7.gif)

## Install

First clone this repo on your local machine

Then navigate to the folder, install dependencies

```bash
npm install
```

Copy `.env-example` into a new file named `.env` and add your ChatGPT email and password.

###### Run the server

First navigate to the directory of this repo on your machine

Then run the server so the extension can communicate with ChatGPT.
```bash
node server.js
```

This will automate interaction with ChatGPT through a headless Chrome browser, thanks to the [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api) library. You will see the browser pop up after running your server. It should automatically log you in, but you may need to manually solve a captcha to complete the process.

###### Add the extension

1. Go to about:addons in your Firefox browser
4. Drag in your xpi file in `chatgpt-firefox-extension/extension/chatgpt-extension-firefox.xpi` 

You'll now see "Ask ChatGPT" if you right click in any text input or content editable area.

## Troubleshooting

If ChatGPT is taking a very long time to respond or not responding at all then it could mean that their servers are currently overloaded. You can confirm this by going to [chat.openai.com/chat](https://chat.openai.com/chat) and seeing whether their website works directly.


## Related

Huge thanks to <a href="https://twitter.com/transitive_bs">Travis Fischer</a> for creating [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)

## License

MIT © Gabe Ragland (follow me on <a href="https://twitter.com/gabe_ragland">Twitter</a>)
