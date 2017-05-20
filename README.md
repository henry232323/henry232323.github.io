<div id="header">
  <a class="button is-success" href="https://discord.gg/UYJb8fQ">Support Server</a>
  <a class="button is-success" href="https://discordapp.com/oauth2/authorize?client_id=305177429612298242&amp;scope=bot&amp;permissions=322625">Add the Bot</a>
  <a class="button" href="https://github.com/henry232323/RPGBot">
      <span class="icon">
        <i class="fa fa-github"></i>
      </span>
      <span>GitHub</span>
    </a>
</div>

<h1 id="whatisrpgbot">What is RPGBot?</h1>

<p>A Bot for assisting with RPG made by <strong>Henry#6174</strong>, with a working inventory, market and economy, team setups and characters aswell. Each user has a server unique inventory and balance. Players may list items on a market for other users to buy. Users may create characters with teams from Pokemon in their storage box. Server administrators may add and give items to the server and its users.</p>

<p><a href=""><strong>Support Server</strong></a></p>

<div id="help">
  <h1 id="help">Help</h1>

  <h2 id="characters">Characters:</h2>

  <ul>
  <li><p><em>allchars</em>   List all guild characters</p></li>

  <li><p><em>character</em>  Get info on a character - <code>rp![character|c|char] &lt;name&gt;</code></p>

  <ul>
  <li><em>create</em>      Create a new character <code>rp!character [create|new] &lt;name&gt;</code></li></ul>

  <p>Example Characters:</p>

  <pre><code>Henry: rp!character create James
  RPGBot: Describe the character (Relevant character sheet)
  Henry: I work for team rocket trying to steal ash's pikachu
  RPGBot: What level is the character?
  Henry: 52
  RPGBot: Any additional info? (Add a character image using the image keyword. Formats use regular syntax i.e image: http://image.com/, hair_color: blond, nickname: Kevin (Separate keys with commas or newlines)
  Henry: hair_color: purple, wealth: im actually rich, eye_color: blue
  RPGBot: Character created! pb!team addmember to add to your characters team!
  </code></pre>

  <ul>
  <li><em>delete</em>      Delete a character of the given name (you must be the owner) <code>rp!character [delete|remove] &lt;name&gt;</code></li></ul></li>

  <li><p><em>characters</em> List all your characters <code>rp![characters|chars]</code></p></li>
  </ul>

  <h2 id="economy">Economy:</h2>

  <ul>
  <li><p><em>bid</em>        Place a bid on the current bidding item in the channel</p></li>

  <li><p><em>economy</em>    Check your or another users balance <code>rp![economy|bal|balance|eco|e] [member]
  </code></p>

  <p><ul>
  <li><em>givemoney</em>   Give the members money (Moderators) <code>rp!economy [givemoney|give] &lt;amount&gt; [members...]</code></li></p>

  <p><li><em>setbalance</em>  Set the balance of the given members to an amount <code>rp!economy [setbalance|set] &lt;amount&gt; [members...]</code></li></ul>

  <p></p></li></p>

  <p><li><p><em>lootbox</em>    List the current lootboxes <code>rp![lootbox|lb]</code></p></p>

  <p><ul>
  <li><em>buy</em>         Buy a lootbox of the given name <code>rp!lootbox buy &lt;name&gt;</code></li></p>

  <p><li><em>create</em>      Create a new lootbox, under the given <code>name</code> for the given cost. 
  Use <code>{item}x{#}</code> notation to add items with {#} weight.
  Weight being an integer. For example with
  <code>bananax2 orangex3</code>: The outcome of the box will be
  a random choice from [banana, banana, orange, orange, orange]
  <code>rp!lootbox [create|new] &lt;name&gt; &lt;cost&gt; [items...]</code></li></p>

  <p><li><em>delete</em>      Delete a lootbox with the given name <code>rp!lootbox [delete|remove] &lt;name&gt;</code></li></ul></p>

  <p></li></p>

  <p><li><p><em>lotto</em>      List the currently running lottos. <code>rp![lotto|lottery]</code></p></p>

  <p><ul>
  <li><em>enter</em>         Enter the lottery with the given name. <code>rp!lotto [enter|join] &lt;name&gt;</code></li></p>

  <p><li><em>new</em>           Create a new lotto, with jacpot payout lasting time in seconds <code>rp!lotto [new|create] &lt;name&gt; &lt;jackpot&gt; &lt;time&gt;</code></li></ul></p>

  <p></li></p>

  <p><li><p><em>market</em>     View the current market listings <code>rp![market|m|pm]</code></p></p>

  <p><ul>
  <li><em>buy</em>           Buy a given amount of an item from the player market at the cheapest given price <code>rp!market [buy|purchase] &lt;id&gt;</code></li></p>

  <p><li><em>create</em>        Create a new market listing <code>rp!market [create|createlisting|new|listitem|list] &lt;cost&gt; &lt;amount&gt; &lt;item&gt;</code></li></p>

  <p><li><em>search</em>        Search the market for an item <code>rp!market search &lt;item&gt;</code></li></ul></p>

  <p></li></p>

  <p><li><p><em>pay</em>        Pay another user money <code>rp!pay &lt;amount&gt; &lt;member&gt;</code></p></li></p>

  <p><li><p><em>shop</em>       Get all items currently listed on the server shop</p></p>

  <ul>
  <li><p><em>additem</em>       Add an item to the server shop, to make an item unsaleable or unbuyable set their respective values to 0</p>

  <pre><code>Henry: rp!shop additem pokeball
  RPGBot: Say 'cancel' to cancel or 'skip' to skip a step. How much should this be buyable for? 0 for not buyable
  Henry: 0
  RPGBot: How much should this be sellable for? 0 for not sellable
  Henry: 10
  RPGBot: What is the minimum level a user must be for this item? 0 for no minimum
  Henry: 0
  RPGBot: Guild shop updated
  </code></pre>

  <p>Can be sold for 10 and cannot be bought. User can be any level. Must be an existing item! Requires Bot Moderator or Admin <code>rp!shop [additem|add] &lt;name&gt;</code></p></li>

  <li><p><em>buy</em>           Buy an item from the shop <code>rp!shop buy &lt;item&gt; &lt;amount&gt;</code></p></li>

  <li><p><em>removeitem</em>    Remove a listed item. Requires Bot Mod or Bot Admin <code>rp!shop removeitem &lt;name&gt;</code></p></li>

  <li><p><em>sell</em>          Sell an item to the shop <code>rp!shop sell &lt;item&gt; &lt;amount&gt;</code></p></li></ul>

  <p></li></p>

  <p><li><p><em>startbid</em>   Start a bid for an item <code>rp!startbid &lt;item&gt; &lt;amount&gt; &lt;startbid&gt;</code></p></li>
  </ul></p>

  <h2 id="groups">Groups:</h2>

  <ul>
  <li><p><em>guild</em>      Get info on a member's guild. Subcommands for guild management</p>

  <ul>
  <li><p><em>create</em>         Create a new guild <code>rp!guild create &lt;name&gt;</code></p>

  <p>Example Usage:</p>

  <pre><code>Henry: rp!guild create Team Rocket
  RPGBot: 'cancel' or 'skip' to cancel creation or skip a step. Describe the Guild (guild description)
  Henry: We are the coolest cats in town, just looking to steal some Pikachus
  RPGBot: Is this guild open to everyone? Or is an invite necessary? (yes or no, no is assumed)
  Henry: yes
  RPGBot: If you'd like give a URL to an image for the guild
  Henry: http://cdn.bulbagarden.net/upload/thumb/d/d3/Team_Rocket_anime.png/300px-Team_Rocket_anime.png
  RPGBot: Finally, you can also set an icon for the guild
  Henry: https://www.seti.soton.ac.uk/static/uploads/socialgroupicon_36_1265776899.gif
  RPGBot: Guild successfully created!
  </code></pre></li>

  <li><p><em>delete</em>         Delete your guild</p></li>

  <li><p><em>deposit</em>        Deposit an amount of money into the guild bank <code>rp!guild deposit &lt;amount&gt;</code></p></li>

  <li><p><em>deposititems</em>   Deposit items into the guild's storage, uses {item}x{#} notation (i.e. bananax3) <code>rp!guild deposititems [items...]</code></p></li>

  <li><p><em>info</em>           Get info on a guild <code>rp!guild info &lt;name&gt;</code></p></li>

  <li><p><em>invite</em>         Invite a user your closed guild <code>rp!guild invite &lt;user&gt;</code></p></li>

  <li><p><em>join</em>           Join a guild (if you have an invite for closed guilds) <code>rp!guild join &lt;name&gt;</code></p></li>

  <li><p><em>kick</em>           Kick a member from a guild <code>rp!guild kick &lt;user&gt;</code></p></li>

  <li><p><em>leave</em>          Leave your guild</p></li>

  <li><p><em>setdescription</em> Set the guild's description <code>rp!guild [setdescription|setdesc] &lt;description&gt;</code></p></li>

  <li><p><em>seticon</em>        Set the guild's icon <code>rp!guild seticon &lt;url&gt;</code></p></li>

  <li><p><em>setimage</em>       Set the guild's image <code>rp!guild setimage &lt;url&gt;</code></p></li>

  <li><p><em>setmod</em>         Give the listed users mod for your guild (guild owner only) <code>rp!guild setmod [members...]</code></p></li>

  <li><p><em>toggleopen</em>     Toggle the Guilds open state</p></li>

  <li><p><em>withdraw</em>       Take money from the guild bank <code>rp!guild withdraw &lt;amount&gt;</code></p></li>

  <li><p><em>withdrawitems</em>  Withdraw items from the guild (guild mods only, same syntax as deposit items) <code>rp!guild withdrawitems [items...]</code></p></li></ul></li>

  <li><p><em>guilds</em>     List guilds</p></li>
  </ul>

  <h2 id="inventory">Inventory:</h2>

  <ul>
  <li><em>inventory</em>  Check your or another users inventory. <code>rp![inventory|i|inv] [member]</code>


  <ul>
  <li><em>give</em>           Give items ({item}x{#}) to a member; ie: ;give @Henry#6174 pokeballx3 <code>rp!inventory give &lt;other&gt; [items...]</code></li>

  <li><em>giveitem</em>       Give an item to a person (Not out of your inventory, must be Bot Moderator) <code>rp!inventory giveitem &lt;item&gt; &lt;num&gt; [members...]</code></li>

  <li><em>takeitem</em>       Remove an item from a person's inventory (Must be Bot Moderator) <code>rp!inventory [takeitem|take] &lt;item&gt; &lt;num&gt; [members...]</code></li></ul>
  </li>
  </ul>

  <h2 id="misc">Misc:</h2>

  <ul>
  <li><p><em>donate</em>     Donation information</p></li>

  <li><p><em>feedback</em>   Give me some feedback on the bot <code>rp!feedback &lt;feedback&gt;</code></p></li>

  <li><p><em>info</em>       Bot Info</p></li>

  <li><p><em>ping</em>       Test the bot's connection ping</p></li>

  <li><p><em>rtd</em>        Roll a number of dice with given sides (ndx notation)
  Example: rp!rtd 3d7 2d4
  Optional Additions:
  Test for success by adding a >/&lt;#</p>

  <p>Grab the top n rolls by adding ^n</p>

  <p>Add to the final roll by just adding a number (pos or neg)</p>

  <p>Examples of all:</p>

  <pre><code>Henry: rp!rtd 8d8 -12 15 ^4 &gt;32
  RPGBot: Roll failed (30 &gt; 32) ([8 + 7 + 6 + 6] + -12 + 15) (Grabbed top 4 out of 8)
  </code></pre>

  <p><code>rp![rtd|rollthedice|dice] [dice...]</code></p></li>

  <li><p><em>source</em>     Displays my full source code or for a specific command.
                 To display the source code of a subcommand you have to separate it by
                 periods, e.g. tag.create for the create subcommand of the tag command.
  <code>rp!source [command]</code></p></li>

  <li><p><em>totalcmds</em>  Get totals of commands and their number of uses</p></li>
  </ul>

  <h2 id="pokemon">Pokemon:</h2>

  <ul>
  <li><p><em>box</em>        Check the pokemon in your box <code>rp!box [member]</code></p></li>

  <li><p><em>pokemon</em>    Subcommands for Pokemon management, see rp!help pokemon. Same use as rp!box <code>rp![pokemon|p] [member]</code></p>

  <ul>
  <li><p><em>create</em>         Create a new Pokemon to add to your box <code>rp!pokemon [create|new]</code></p>

  <p>Example Usage:</p>

  <pre><code>Henry: rp!pokemon create
  RPGBot: In any step type 'cancel' to cancel. What will its nickname be?
  Henry: Charry
  RPGBot: What species of Pokemon is it?
  Henry: Charizard
  RPGBot: In any order, what are its stats? (level, health, attack, defense, spatk, spdef)For example level: 5, health: 22, attack: 56 Type 'skip' to skip.
  Henry: level: 23, health: 42, attack: 52, spdef: 12, health: 88, spatk: 88
  RPGBot: Any additional data? (Format like the above, for example nature: hasty, color: brown)
  Henry: nature: adamant, color: shiny
  RPGBot: Finished! Pokemon has been added to box with ID 1
  </code></pre></li>

  <li><p><em>info</em>           Get info on a Pokemon <code>rp!pokemon info &lt;id&gt;</code></p></li>

  <li><p><em>trade</em>          Offer a trade to a user.
  <code>your_id</code> is the ID of the Pokemon you want to give, <code>their_id</code> is the Pokemon you want from them.
  <code>other</code> being the user you want to trade with <code>rp!pokemon trade &lt;your_id&gt; &lt;their_id&gt; &lt;other&gt;</code></p></li>

  <li><p><em>release</em>        Release a Pokemon from your box <code>rp!pokemon [release|delete|rm|remove] &lt;id&gt;</code></p></li></ul></li>
  </ul>

  <h2 id="settings">Settings:</h2>

  <ul>
  <li><p><em>settings</em>   Get the current server settings <code>rp![settings|s|configuration|conf]</code></p>

  <ul>
  <li><em>additem</em>        Add a custom item <code>rp!settings additem &lt;name&gt;</code></li></ul>

  <p>Example Usage:</p>

  <pre><code>Henry: rp!s additem Banana
  RPGBot: Describe the item (a description for the item)
  Henry: A delicious yellow fruit
  RPGBot: Additional information? (Attributes formatted in a list i.e `color: 400, value: 200`)
  Henry: color: yellow, taste: delicious, type: fruit
  RPGBot: Item successfully created
  </code></pre>

  <ul>
  <li><em>iteminfo</em>       Get info on a server item <code>rp!settings iteminfo &lt;item&gt;</code></li>

  <li><em>items</em>          See all items for a guild</li></ul></li>
  </ul>

  <h2 id="team">Team:</h2>

  <ul>
  <li><em>team</em>       Check a character's team <code>rp!team &lt;character&gt;</code>


  <ul>
  <li><em>add</em>            Add a Pokemon to a character's team <code>rp!team [add|addmember] &lt;character&gt; &lt;id&gt;</code></li>

  <li><em>remove</em>         Remove a Pokemon from a character's team <code>rp!team [remove|removemember] &lt;character&gt; &lt;id&gt;</code></li></ul>
  </li>
  </ul>

  <h2 id="user">User:</h2>

  <ul>
  <li><em>userinfo</em>   Get info on a user <code>rp![userinfo|ui] [user]</code></li>

  <li><em>experience</em> Get your or another user's level information. Help on this command for experience subcommands
  EXP is calculated using a 0.1x^2+5x+4 where x is equal to the user's current level
  Spamming commands or messages will not earn more exp! <code>rp![experience|exp] [member]</code>


  <ul>
  <li><em>add</em>         Give the given members an amount of experience <code>rp!experience add &lt;amount&gt; [members...]</code></li>

  <li><em>setlevel</em>    Set the given members level <code>rp!experience setlevel &lt;level&gt; [members...]</code></li></ul>
  </li>
  </ul>
</div>

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="https://raw.githubusercontent.com/jgthms/bulma/master/css/bulma.css">
<style>
</style>
