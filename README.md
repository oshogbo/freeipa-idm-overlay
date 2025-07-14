# Why?

Vermaden has written an excellent blog post explaining why this is important for Kerberos authentication.
No matter how much detail I include here, it would still be better for you to check out the [post](https://vermaden.wordpress.com/2024/06/23/freebsd-samba-share-freeipa-idm-auth/)
directly.

# Build

```
poudriere ports -c -U https://github.com/oshogbo/freeipa-server-overlay.git -p freeipa_server_overlay
poudriere bulk -p <port> -O freeipa_server_overlay -j <jail> net/freeipa-client
```
