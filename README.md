const Discord = require('discord.js');
const client = new Discord.Client();

const token = ('NjY5OTcyMDg4MjkxMDY1ODY4.XinmMg.xUACIMJc0QJSLtDEhZJLNMPAPCE');

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
})

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('Pong!');
  }
})

client.login(token);
