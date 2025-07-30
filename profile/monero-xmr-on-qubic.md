# Monero (XMR) on Qubic
The [Qubic Monero PoC](https://qubic.org/blog-detail/outsourced-computations-a-step-toward-decentralized-ai-innovation) enables you to mine Monero (XMR) on the Qubic network.

Normally only 50% of the time XMR mining is enabled. To fully support Qubic we offer you an easy way to connect with the [QLI Client](https://github.com/qubic-li/client/).
The client manages your CPU resources optimal, it switches automatically between Qubic AI Training and XMR mining.

## Short Path
1. Create a Qubic Id/Address: [docs.qubic.org/learn/wallets](https://docs.qubic.org/learn/wallets)
2. Connect to Qubic XMR: `stratum+tcp://xmr.qubic.li:3333` with your Qubic Address
3. Monitor on [pool.qubic.li](https://pool.qubic.li)
4. Earn Qubic's

> [!CAUTION]
> Your XMR contributions are only counted during Qubic Custom Minign Phase (every ~15min for ~15min) or during [XMR Marathon](#the-marathon)

## The Marathon
Every Saturday from 12 UTC to Sunday 12 UTC, Qubic dedicates 24h to the Monero (XMR) PoC.

During this time, all your XMR contributions count towards the revenue.

> [!TIP]
> Use the marathon time to connect all your rigs to Qubic XMR without interruption

## How can i connect?
To monitor your activity: [pool.qubic.li](https://pool.qubic.li)

1. Using [QLI Client](https://github.com/qubic-li/client/) to fully leverage Qubic + Custom Mining (XMR)
2. Using any Monero (XMR) / RandomX compatible miner which support the stratum protocol (e.g. [XMRig](https://xmrig.com/))
3. Using services like [MiningRigRental](https://www.miningrigrentals.com/) or [Nicehash](nicehash.com)
4. Using Proxy/Bridges like [XMRig Proxy](https://xmrig.com/proxy)

We recomend you to create an account on [pool.qubic.li](https://pool.qubic.li) to have full control of everything. If you don't want to share an e-mail address or you like to stay completely anon, you can also join with just a Qubic Address. In any case, you need a Qubic Address/Id.

Create an address with one of the available wallets: https://docs.qubic.org/learn/wallets

### Pool Addresses
For easyness use one of the following Pool Addresses:

|  Location 	|  TCP | SSL/TLS 	|  Comments |
|---	|---	|--- |---	|
|  EU/World  	|  stratum+tcp://xmr.qubic.li:3333 |  stratum+ssl://xmr.qubic.li:3334 |  EU |
|  HK 	|  stratum+tcp://hk.xmr.qubic.li:3333 |  stratum+ssl://hk.xmr.qubic.li:3334	|  Hong Kong |
|  US 	|  stratum+tcp://us.xmr.qubic.li:3333 |  stratum+ssl://us.xmr.qubic.li:3334	|  New York |
|  SG 	|  stratum+tcp://sg.xmr.qubic.li:3333 |  stratum+ssl://sg.xmr.qubic.li:3334	|  Singapore |

### How To Start XMRig
Linux:
- `xmrig --url "stratum+tcp://xmr.qubic.li:3333" -u QUBICADDRESS`
- `xmrig --url "stratum+tcp://xmr.qubic.li:3333" -u QLI_ACCESS_TOKEN`

Windows:
- `xmrig.exe --url "stratum+tcp://xmr.qubic.li:3333" -u QUBICADDRESS`
- `xmrig.exe --url "stratum+tcp://xmr.qubic.li:3333" -u QLI_ACCESS_TOKEN`

Example: `xmrig.exe --url "stratum+tcp://xmr.qubic.li:3333" -u VAVZCPHUDJEZXCQXYOOOBIKJQHWBVKZMLUDCPEFDEEZKGZJQMJYGSUMDRYQZ`

Optional you can pass a rig name with `--rig-id="MySuperRig"`

### How To Add A Pool In Mining Rig Rentals
<img width="500" alt="mrr-pool-sample" src="https://github.com/user-attachments/assets/261982ec-4429-4b35-8d40-2207df04b430" />
1. Give your pool a name
2. Add the pool address: `xmr.qubic.li:3333`
3. Add the worker name: `QUBICADRESSS` or `QLI_ACCESS_TOKEN` or `QLI_USERID`
4. The password can be left empty
