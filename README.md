# Uniswap Labs: Front End Interfaces

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/domwoe/interface)

An open source repository for all Uniswap front end interfaces maintained by Uniswap Labs. Uniswap is a protocol for decentralized exchange of Ethereum tokens.

## 🚀 Deploying on ICP

Add a `dfx.json` config file:

```bash
touch dfx.json
```

Add the following content to the `dfx.json` file:

```json
{
  "canisters": {
    "interface": {
      "frontend": {
        "entrypoint": "apps/web/build/index.html"
      },
      "source": ["apps/web/build"],
      "type": "assets"
    }
  },
  "version": 1
}
```

Build the web app:

```bash
yarn web build:production
```

Deploy the web app:

```bash
dfx deploy --playground
```

## Interfaces

- Web: [app.uniswap.org](https://app.uniswap.org)
- Wallet: [wallet.uniswap.org](https://wallet.uniswap.org)

## Socials / Contact

- Twitter: [@Uniswap](https://twitter.com/Uniswap)
- Reddit: [/r/Uniswap](https://www.reddit.com/r/Uniswap/)
- Email: [contact@uniswap.org](mailto:contact@uniswap.org)
- Discord: [Uniswap](https://discord.gg/FCfyBSbCU5)

## Uniswap Links

- Website: [uniswap.org](https://uniswap.org/)
- Docs: [uniswap.org/docs/](https://docs.uniswap.org/)

## Whitepapers

- [V3](https://uniswap.org/whitepaper-v3.pdf)
- [V2](https://uniswap.org/whitepaper.pdf)
- [V1](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Apps

For instructions per application or package, see the README published for each application:

- [Web](apps/web/README.md)
- [Mobile](apps/mobile/README.md)

## Releases

All interface releases are tagged and published to this repository. To browse them easily, see the [Github releases tab](https://github.com/Uniswap/interface/releases).

## Translations

Translations for our applications are done through [crowdin](https://crowdin.com).

| App     | Coverage |
| ------- | -------- |
| web     | [![Crowdin](https://badges.crowdin.net/uniswap-interface/localized.svg)](https://crowdin.com/project/uniswap-interface) |
| mobile  | [![Crowdin](https://badges.crowdin.net/uniswap-wallet/localized.svg)](https://crowdin.com/project/uniswap-wallet) |

## 🗂 Directory Structure

| Folder      | Contents                                                                       |
| ----------- | ------------------------------------------------------------------------------ |
| `apps/`     | The home for each standalone application.                                      |
| `config/`   | Shared infrastructure packages and configurations.                             |
| `packages/` | Shared code packages covering UI, shared functionality, and shared utilities.  |
