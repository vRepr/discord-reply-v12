
**Discord Reply v12 | vRepr**

**NPM:** https://npmjs.com/package/discordv-reply-v12

**Discord:** vRepr#0001

**Please Note:** This code was taken from (https://github.com/SykoCoder1/discord-replys) and was tweaked to work with the package *discord-buttons*.
                 Furthermore, I take no credit for this code and only did this with the sole intention to fix an issue I had.

# Example

```
const Discord = require("discord.js");
const client = new Discord.Client();
require("discord-reply-v12");

client.on('message', async message => {
  if (message.content === "vRepr") {
    message.replyMention("vRepr")//Mention Reply

    message.replyNoMention("vRepr")//No Mention Reply
  }

});
```

## Embed

```
const Discord = require("discord.js");
const client = new Discord.Client();
require("discord-reply-v12");

client.on('message', async message => {
  if (message.content === "vRepr") {

  let embed = new discord.MessageEmbed()
  .setTitle("vRepr | İnline Reply Message")
  .setDescription(`Test Reply Message`)


    message.replyMention(embed)//Mention Reply

    message.replyNoMention(embed)//No Mention Reply
  }

});
```

 ## Installation

```
npm i discord-reply-v12
```