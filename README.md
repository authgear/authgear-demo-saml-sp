# Authgear E2E SAML SP

This branch is for QA e2e test.

https://authgear-saml-e2e-sp.pandawork.com

## Development

Assume you have python3 installed globally on your machine, or
you are a user of https://github.com/nix-community/nix-direnv

```sh
make -C demo-flask setup
make -C demo-flask start
```

## Deploying to Pandawork

```sh
make -C demo-flask push-image
make -C deploy deploy
```
