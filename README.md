Installation

If you have trouble with the installation, please feel free to visit our discord address.


# Define Module & Client

Make a ne file in you bot andd name it bonify.js

``const Discord = require("discord.js");
const client = new Discord.Client();
const vBonify = require("./bonify.js");
const dbl = new vBonify("TOKEN-HERE", client);


client.login("MTk4NjIyNDgzNDcxOTI1MjQ4.Cl2FMQ.ZnCjm1XVW7vRze4b7Cq4se7kKWs");
``

# Server Count & Shard Count Posting
``
client.on("ready", async () => {
  dbl.serverCount();
  /* 
  -> Server count posted. 
  or 
  -> Server count & shard count posted.
  */

});``

# Vote Checking


``let hasVote = await dbl.hasVoted("714451348212678658"); // -> User ID
  if(hasVote === true) {
      console.log("Voted")
    } else {
      console.log("Vote please.")
  }
// -> Vote please.``


# Search on Bonify
``let botFind = await dbl.search("779641401482805289");
console.log(botFind.username) // -> Allegro``
