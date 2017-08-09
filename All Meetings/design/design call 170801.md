# Design call notes 8/1/17

Attendance: Andrei, Anna, Jarrad, Vic

andmironov [12:57 PM] 

Hey guys, here’s a brief recap of today’s design-related talk

_TODO_

*Main Screen*
- Add `Manage Assets` screen;
- Add Banner when there are no assets to display;

*Value Screen*
This is the screen with the graph visualising the asset’s value change . Not sure if it’s necessary at all;

*Token Data Screen*
- Swap `My TOKEN` and `Market value`;
- What is the Graph visualising?

*QR Screen*
- Add label to Address field;
- Add `Send` button (send via Status);
- Add `Testnet` warnings when somebody’s sharing their address;

*Request Transaction*
Finish this screen, considering all changes in the `Share QR Screen`

*Send Transaction Screen*
- Swap `Choose Recipient` and `Specify Amount`, add all necessary changes accordingly;
- Add a button to browse file system for QR codes;
- Add error states when there’s an invalid QR or address;
- Consider renaming `Done` to `Save`;
- Rename `Confirm` to `Sign`;
- Add new look to password field to make it more secure and harder to replicate;
- Consider moving `Cancel` to the bottom;
- Display the total transaction fee on `Transaction Fee Screen` (in Wei or in ETH);
- Add name/face to recipient address when available;
- `Date and time` is actually `Block number`, rename it and add screen;
- Add `Testnet` warnings;

*Transaction History*
- Rename `Pending` to `Unsigned`;
- Add `Future Transactions` and `Pending transactions` to the transaction history list;
- Add filter by `Incoming/Outgoing` and `Date and Time`;
- Think on how to display the secure input when confirming multiple transactions at the same time;

*Transaction Details*
- Add confirmation progress. If there are more than 12 confirmations than the transaction is considered secure.

_Other things worth mentioning_
- Think more about updates to the `/send` command. What are the benefits of using it In favour of the built-in wallet?;
- Update the profile (Address sharing and add a way to register a username);
- Think more about the new nav and what are we going to do with the Discover screen;
