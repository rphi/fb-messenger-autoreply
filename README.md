# Facebook Messenger Autoreply Bot

A simple NodeJS app to let people know you don't use Messenger, and that
they should try on better platforms.

Messaging `/stop` in a thread disables the bot, `/resume` removes that
thread from the whitelist. Group chats are automatically whitelisted.

The personal thread whitelist isn't persisted (currently).

This makes use of the very handy [facebook-chat-api](https://github.com/Schmavery/facebook-chat-api/) Node module.

## Usage

Copy the `credentials.js.template` file to `credentials.js` include your 
FB username and password. (Remember not to post this file online,
`.gitignore` should exclude it.)

It doesn't like two factor.

Run `npm install` and `npm start` in the project root.