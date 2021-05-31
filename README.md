# InlineReplies.JS
InlineReplies.JS is a library that extends discord.js version 12 to add inline replies.

## Setup
All you have to do is import it and set some settings when you define client, then everything will work flawlessly and you'll have access to the `message.inlineReply()` function.

## Example
```js
const { Client } = require("discord.js");

require("inlinereplies.js");

const client = new Client({
    allowedMentions: {
        // set repliedUser value to `false` to turn off the mention by default
        repliedUser: true
    }
});

client.on("message", message => {
    if (message.author.bot) return;
    if (message.content === "example") {
        message.inlineReply("Hi, this is an example of inlineReplies.JS!");
    }
});

client.login("Your bot token");
```

## Contribution
If you want to contribute, make your changes to the `index.js`, then go ahead and make a PR, then we will look at the code and merge it.

## Licensing
MIT License

## Donate
If you want to donate, you can donate 5 USD or 10 USD, just go to [here](https://discord.com/users/763767239018938368), then send nitro or nitro classic to the user.

## Thanks :D