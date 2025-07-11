# Why?

TODO.

# Build

```
poudriere ports -c -U https://github.com/oshogbo/freeipa-server-overlay.git -p freeipa_server_overlay
poudriere bulk -p <port> -O freeipa_server_overlay -j <jail> net/freeipa-client
```
