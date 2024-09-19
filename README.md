# whatsapp-gpt-fix
---
## While trying to run whatsapp-gpt I firstly got the following error:

```
10:09:20.723 [Client/Socket DEBUG] Dialing wss://web.whatsapp.com/ws/chat
10:09:20.975 [Client/Socket DEBUG] Frame websocket read pump starting 0x140001f24d0
10:09:23.120 [Client/Recv DEBUG] <failure location="cco" reason="405"/>
10:09:23.120 [Client ERROR] Client outdated (405) connect failure
10:09:23.121 [Client/QRChannel DEBUG] Closing channel with status {Event:err-client-outdated Error:<nil> Code: Timeout:0s}
Login event: err-client-outdated
10:09:23.122 [Client/Socket ERROR] Error reading from websocket: websocket: close 1006 (abnormal closure): unexpected EOF
10:09:23.122 [Client/Socket DEBUG] Frame websocket read pump exiting 0x140001f24d0
10:09:23.122 [Client DEBUG] OnDisconnect() called, but it was expected, so not emitting event
```

Fix to that is just upgrading your packages by running ```go get -u ./...``` in your terminal.
