# Planning call notes 02/10/17

Attendance: Jarrad, Andrei, Anna, Goran, Eric, Vic, Adam, Anastasya, Ewetumo, Frank, Jan, Ivan D, Oskar, Roman

### TL;DR; Approved scope for the Devcon3 release - Wallet, Network Switching, Discover, Push Notification 1-to-1. Keep using Infura for now.

- discussion about features we can package for Devcon3: Wallet, Discover, Network Switching, Push Notifications(with the minimum user story)

*Wallet*
- Wallet should be good unless any developer objeciton that it's not feasible to include this to thre release
- New wallet is centralized though (the Dapp wasn’t?), but we can make it configurable and add chat bots to support decentralization - follow up with requirements update.  For the Devcon3 - just keep existing scope
- Finalize Wallet design decision for the /send command
- TestTeam is going to test Wallet, and pending PRs

*Network Switching*
- Network switching - we have issues and we won’t be able to fix this soon.  Just create the message and restart the app.  Clarify the list of networks.  It seems doable in a week.  What are the networks in the list? Ideally to have all 3 networks, but the main net is under question.
- Network switching - all networkds  with upstream RPC
- Network switching - how the dapps list will change? We can ignore it for Devcon3 scope.

*Discover*
- Discover - is pretty feasible to include to Devcon3, open issue is how to enable the new feature (flag?) or keep working in the branch. Goran was working alone on this and now cando in parallel (Oskar can join the squad)
- Discover - revisit Dapps list and make sure they work
- Dapps list is static now.  How we distinguish dapps from contacts?

*Push Notifications*
- Push notifications - good to have the minimum story by Devcon3 and POC for mailbox (PSS maybe instead of Whisper? both are pretty experimental)
- Firebase analytics should be removed

*Workflow*
- we want to switch to the time based development and commit to develop new features and go away from the branch based features
- squads vs. working groups - dynamic groups can be better that long term groups.  Me might want to have more squads on go-side (edited)
- Need more stability on the go-side
- We have requirements issues still - can we instead of raise the issues just try to solve them (or limit the scope)?
- we’re still not aligned on our approach to requirements management

*status-go*
- geth 1.7 rebase seems to be ready but do we need it for Devcon3? We can drop it from Devcon3 scope.
- keep Infura for the Devcon3 scope
