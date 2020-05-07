Padavan CI
===

```
# replace :token, :user, and :repo
curl -H "Authorization: token :token" \
    -H 'Accept: application/vnd.github.everest-preview+json' \
    "https://api.github.com/repos/:user/:repo/dispatches" \
    -d '{"event_type": "build", "client_payload": {"target": "MI-MINI K2P", "config": "CONFIG_FIRMWARE_INCLUDE_HTTPS=y CONFIG_FIRMWARE_INCLUDE_OPENSSL_EXE=y"}}'
```