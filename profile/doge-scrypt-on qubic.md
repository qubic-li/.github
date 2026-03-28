# Dogecoin (DOGE) on Qubic

The [Qubic Dogecoin Integration](https://qubic.org/blog-detail/outsourced-computations-a-step-toward-decentralized-ai-innovation) enables you to mine Dogecoin (DOGE) on the Qubic network.

With 100% AI Training and at the same time Doge mining, Qubic offers a unique experience.

## Short Path

1. Create a Qubic Id/Address: [docs.qubic.org/learn/wallets](https://docs.qubic.org/learn/wallets)
2. Connect to Qubic DOGE: `stratum+tcp://doge.qubic.li:12480` with your Qubic Address
3. Monitor on [pool.qubic.li](https://pool.qubic.li)
4. Earn Qubic's

> [!CAUTION]
> This is currently for testing only. We estimage the official start in the beginning of april.

## How can I connect?

To monitor your activity: [pool.qubic.li](https://pool.qubic.li)

1. Using any Dogecoin (DOGE) / Scrypt compatible miner which supports the stratum protocol (e.g. [BFGMiner](http://bfgminer.org/), [CGMiner](https://github.com/ckolivas/cgminer))
2. Using services like [MiningRigRentals](https://www.miningrigrentals.com/) or [NiceHash](https://nicehash.com)
3. Using Proxy/Bridges like [Stratum Proxy](https://github.com/slush0/stratum-mining-proxy)

We recommend you to create an account on [pool.qubic.li](https://pool.qubic.li) to have full control of everything. If you don't want to share an e-mail address or you like to stay completely anon, you can also join with just a Qubic Address. In any case, you need a Qubic Address/Id.

Create an address with one of the available wallets: https://docs.qubic.org/learn/wallets

### Pool Addresses

For easiness use one of the following Pool Addresses:

| Location | Address | Comments |
|---|---|---|
| World | stratum+tcp://doge.qubic.li:12480 |  |

### How To Start Mining

Linux:
- `cgminer --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QUBICADDRESS`
- `cgminer --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QLI_ACCESS_TOKEN`

Windows:
- `cgminer.exe --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QUBICADDRESS`
- `cgminer.exe --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QLI_ACCESS_TOKEN`

Example: `cgminer.exe --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u VAVZCPHUDJEZXCQXYOOOBIKJQHWBVKZMLUDCPEFDEEZKGZJQMJYGSUMDRYQZ`

Optionally you can pass a rig name with `--rig-id="MySuperRig"`

### How To Add A Pool In Mining Rig Rentals

1. Give your pool a name
2. Add the pool address: `doge.qubic.li:12480`
3. Add the worker name: `QUBICADDRESS` or `QLI_ACCESS_TOKEN` or `QLI_USERID`
4. The password can be left empty

## QLI Pools Rules

This Pool uses a single payment system.
At the end of each Epoch, your delivered solutions/shares are used to calculate your stake in Epoch+1. Payout is always one week (epoch) after. The Pool fee is max 10%.

### PPS vs. Solo

With the QLI pools you can choose between PPS (Pay Per Share) or solo training. With PPS you avoid the own volatility which is useful for smaller environments. It is also allowed to run some workers as PPS and others as solo training where you will see revenue only when you find valid Qubic Solutions.

### When Payout

Rewards are distributed each Wednesday.
