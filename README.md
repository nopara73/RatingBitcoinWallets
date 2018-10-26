# Rating Bitcoin Wallets

|                                                                               | [Privacy](#i-privacy) | [Trust](#ii-trust) | [Security](#iii-security)                  | [Ease of Use](#ease-of-use) |
|-------------------------------------------------------------------------------|-----------------------|--------------------|--------------------------------------------|-----------------------------|
| Bitcoin Core                                                                  | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Wasabi Wallet                                                                 | &#9745;&#9745;        |                    | &#9745;&#9745;&#9745;                      | &#9745;&#9745;              |
| Hidden Wallet (not in production)                                             | &#9745;&#9745;        | &#9745;            | &#9745;&#9745;&#9745;&#9745;               | &#9745;                     |
| CoinBase                                                                      | &#9745;&#10060;       | &#10060;           | &#9745;&#10060;                            | &#9745;&#9745;&#9745;       |
| Blockchain.info                                                               |                       |                    | &#9745;                                    | &#9745;&#9745;&#9745;       |
| Blockchain.info + SharedCoin (not in production)                              | &#9745;               |                    | &#9745;                                    | &#9745;&#9745;&#9745;       |
| Electrum (Desktop)                                                            |                       | &#9745;            | &#9745;&#9745;&#9745;&#9745;               | &#9745;&#9745;              |
| Electrum (Desktop) + Bitcoin Core with Electrum Server                        | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Electrum (Desktop) + Bitcoin Core (through Electrum Personal Server)          | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Trezor                                                                        |                       |                    | &#9745;&#9745;&#9745;                      | &#9745;&#9745;              |
| Trezor + Electrum (Desktop)                                                   |                       | &#9745;            | &#9745;&#9745;&#9745;&#9745;               | &#9745;&#9745;              |
| Trezor + Electrum (Desktop) + Bitcoin Core with Electrum Server               | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Trezor + Electrum (Desktop) + Bitcoin Core (through Electrum Personal Server) | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Mycelium                                                                      |                       |                    | &#9745;&#9745;                             | &#9745;&#9745;&#9745;       |
| Mycelium + ShufflePuff (not in production)                                    | &#9745;               |                    | &#9745;&#9745;                             | &#9745;&#9745;&#9745;       |
| JoinMarket with blockr.io API (not in production)                             | &#9745;               |                    | &#9745;&#9745;&#9745;                      | &#9745;&#9745;              |
| JoinMarket + Bitcoin Core                                                     | &#9745;&#9745;        | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Dark Wallet                                                                   | &#9745;               |                    | &#9745;                                    | &#9745;&#9745;              |
| Bitcoin Knots                                                                 | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Stratis: Breeze Wallet                                                        | &#9745;&#9745;        | &#9745;            | &#9745;&#9745;&#9745;&#9745;               | &#9745;                     |
| Armory                                                                        | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;        |                             |
| Bread Wallet                                                                  |                       | &#9745;            | &#9745;&#9745;&#9745;&#9745;               | &#9745;&#9745;              |
| Paper Wallet (generated offline, spent by imported into a full node)          | &#9745;               | &#9745;&#9745;     | &#9745;&#9745;&#9745;&#9745;&#9745;&#9745; |                             |

If any decision I made here is not clear or you find debatable, please open an issue. 

This writeup is intended to be an improvement on [Jonas Schnelli's](https://github.com/jonasschnelli) Bitcoin wallet triangle, [presented](https://www.youtube.com/watch?v=XORDEX-RrAI&feature=youtu.be&t=3440) at the Building on Bitcoin 2018 conference.

Jonas rated the wallets in three main categories: privacy, trust and security. I expand on these with sub categories, define requirements and I add a new, ease of use category to this.

Beware that, the properties of privacy, trust and security are similar in a sense that, they fail where they are the weakest. This notion limits the reliability of this rating system.

# I. Privacy

## I/a. Blockchain Level Privacy

Can the wallet sufficiently withstand blockchain analysis? (&#9745;/ )

## I/b. Network Level Privacy

- Does the wallet get to know the current state of the blockchain without leaking relevant information to third parties? (&#9745;/ )  
- Is the wallet open source? (&#10060;/ )

# II. Trust

- Full Nodes (&#9745;&#9745;) / SPV nodes (&#9745;) / Centrally Validating Nodes ( )
- Is the wallet open source? (&#10060;/ )

# III. Security

## III/a. Privacy (Hiding)

Hiding (&#9745;/ ) could be another subcategory of Privacy, however it is less relevant from a privacy point of view and more relevant from a security point of view. The criteria for Hiding is, if the wallet runs on a general purpose environment or not. Currently all wallets are such wallets, except hardware wallets.

## III/b. Trust

This subcategory is the same as the Trust main category. This is necessary to include into the Security, because getting tricked by third parties is a direct security risk. Thus we duplicate it, so to denote the interconnectedness of the properties. (&#9745;&#9745; / &#9745; / ) 

### III/c. Key Safety

Is spending from the wallet happens in a...
- cold environment (&#9745;&#9745;&#9745;)
- desktop (&#9745;&#9745;)
- mobile (&#9745;)
- browser ( )
- private keys are not controlled by the user (&#10060;)

# Ease of Use

- Using the wallet is instant and doesn't require initial sync or setup. (&#9745;&#9745;&#9745;)
- Using the wallet is instant, but a bit of initial sync is required or setup. (&#9745;&#9745;)
- Using the wallet requires sync every time when opening it and a bit of initial sync or setup required (&#9745;)
- Using the wallet requires sync every time when opening it and a considerable amount of initial sync or setup is required ( )
