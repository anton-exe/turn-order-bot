# turn-order-bot
T.O.B. is a Discord bot to help keep track of turn orders.

## Usage
To start a thread, run `tob!start [user] [user] ...`, either pinging or putting the user id of everyone you want in the thread. The turn order will be based off the order you put everyone into the command. When you send the command, T.O.B. will start a new Discord thread for all the pings.

To change the thread name, run `tob!rename [name]`.

When it's someone's turn, the bot will ping them every 23 hours, in case they were busy during previous pings.

When your turn is done, run `tob!next`. You can also optionally add arbitrary text that will be sent with every ping, by doing something like `tob!next PS. remember to do XYZ!!`.

To immediatelly send another ping and reset the timer, run `tob!reping`.

If someone already took their turn, but is forgetting to run `tob!next`, you can simply add `force` as an argument to force pass their turn.

To join a thread midway through, run `tob!join [index]`, with the index being where in the order you want to join (Note: List indices start at **0**. Putting "5" in as the index puts you in the 6th position). To leave early, run `tob!leave [index]`.

To check the turn order, run `tob!order`.

Once the thread is done, run `tob!end`.
