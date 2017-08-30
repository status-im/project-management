# Status.im v0.9.10 Release Notes 14/08/2017

# Summary

Completed the Wallet UI redesign mockups and approved iOS and Android screens to handoff for implementation.

Some housekeeping and fixing the development environment and infrastructure services did some important refactoring and tests update. More details in the following [Github issues]( https://github.com/status-im/status-go/issues?utf8=%E2%9C%93&q=is%3Aissue%20164%20178%20179%20196%20205%20208%20224%20234%20221).


# Epic Progress

Here’s to mention the progress on the new features and improvements that we’ve done in this iteration - the following is not done but work in progress.

## Wallet UI Redesign

Work in progress on the `Wallet Redesign` epic.

[#1596](https://github.com/status-im/status-react/pull/1596) PR: Started implementation for the new Wallet UI 

This PR amends main wallet screen with basic navigation to a mocked send transaction screen.
status: wip but ready to merge since we don't render anywhere

[#1556](https://github.com/status-im/status-react/pull/1556) PR: [WIP] Wallet main screens UI


## Network Switching

Work in progress on the `Network Switching` epic, mostly on [#190](https://github.com/status-im/status-go/issues/190) JSON-RPC Server Delegation in Network Configuration



## Smooth/Optimized Usage

[1536](https://github.com/status-im/status-react/issues/1536 )	Utilise CallRPC method from status-go 

By making this change we will stop using Http RPC calls for communication with local geth node. This will simplify resuming application after background mode as well as improve performance and security.



# Bug Fixes

#1015	Message from newly joined participant of public chat is shown not at the end of a chat

#1050	App does not respond to any tap if try to send requested sum with 15 digits after comma

#1051	New message from A is shown in the beginning of a group chat for all other users after user A cleared chat history

#1195	Message from A is shown to B in the beginning of 1-1 chat if chat was deleted by A and started again

#1469	Plain text instead of map is shown to recipient of location command [develop]

#1486	App crashes when chatting with newly added chat right after the Console chat was removed

[List on Github](https://github.com/status-im/status-react/issues?utf8=%E2%9C%93&q=is%3Aissue%201015%201050%201051%201195%201469%201486%201536%20)




# Known Issues

1. For upgraded version: All old send/request/location messages are removed after upgrade, chats contain only text and emojis
2. Crash of old version if new version sends eth to group chat 
3. Crash of old version if new version sends Location command (to 1-1 chat or group chat)

https://github.com/status-im/status-react/issues/989

