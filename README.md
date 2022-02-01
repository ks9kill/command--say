const Discord = require('discord.js');

module.exports = {
  name: "say", 
  alias: ["decir"],

execute (client, message, args){

  let decir = args.join(` `)
  if(!decir){
    return message.channel.send("Debes poner un mensaje para que lo pueda enviar.")
  }
message.channel.send(decir)
message.delete({timeout: 1000})
 }

}
