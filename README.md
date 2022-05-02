client.on('message', message =>{
  if (message.author.id == client.user.id || message.author.bot){
    return;
  }

  if (message.content === "ほのうスライム好き？"){
    let reply_text = "好き";
    message.reply(reply_text)
      .then(message => console.log("Sent message: " + reply_text))
      .catch(console.error);
    return;
  }
});
