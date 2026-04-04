# Dogecoin (DOGE) on Qubic

The [Qubic Dogecoin Integration](https://qubic.org/blog-detail/qubic-dogecoin-mining-transition-plan-april-2026) brings Scrypt ASIC mining to the Qubic network — running **in parallel** with AI training, not replacing it.

Your CPUs/GPUs keep training Aigarth. Your ASICs earn on top. 100% AI + 100% DOGE, simultaneously.

## Quick Start

1. Create a Qubic Id/Address: [docs.qubic.org/learn/wallets](https://docs.qubic.org/learn/wallets)
2. Point your Scrypt miner to: `stratum+tcp://doge.qubic.li:12480`
3. Use your **Qubic Id/Address** as the username
4. Monitor on [platform.qubic.li](https://platform.qubic.li)

## How It Works

1. ASIC miners submit Scrypt (DOGE) shares via stratum
2. Shares are validated on-chain through [Oracle Machines](https://docs.qubic.org/developers/oracles/) — decentralized, not single-pool-operator trust
3. Mined DOGE is sold on the market
4. Proceeds buy back QUBIC (Qubic tokens)
5. QUBIC are distributed to participants based on contribution

**You earn QUBIC, not DOGE.** The Dogecoin generates external revenue that flows back into the Qubic economy.

## Fees & Rewards

### DOGE Mining — 0% Fee
DOGE mining on Qubic is **feeless** during the launch phase. No pool fees, no hidden costs.

**How you earn:** All Dogecoin mined through the network is sold on the market and the proceeds are used to buy back QU. This QU is then distributed to DOGE miners based on their contribution. The more hashrate you bring, the bigger your share.

| Phase | How rewards work |
|---|---|
| **Phase 1 (Testing)** | Rewards in QUBIC are funded by the pool — you earn from day one |
| **Phase 2+ (Full launch)** | Buyback mechanism kicks in. QUBIC rewards can be topped up to ~110% from buyback proceeds. Any surplus is burned. |

### Qubic AI Training (separate)
- Pool fee: max 7% (applies to QUBIC rewards from CPU/GPU AI training only)
- PPS or Solo mode available
- Payouts: Weekly, one epoch after contribution

> DOGE mining and AI training have completely separate fee structures. The 10% pool fee applies only to CPU/GPU based AI training rewards — DOGE mining is feeless.

## How To Connect

### Compatible Hardware
Any Scrypt-compatible ASIC miner works: Antminer L3+, L7, L9, Goldshell Mini-DOGE Pro, and others.

### Pool Address

| Location | Address |
|---|---|
| World (auto detection) | `stratum+tcp://doge.qubic.li:12480` |
| US | `stratum+tcp://us.doge.qubic.li:12480` |
| ASIA | `stratum+tcp://asia.doge.qubic.li:12480` |

### Mining Commands

**Linux:**
```
cgminer --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QUBICADDRESS
```

**Windows:**
```
cgminer.exe --scrypt --url "stratum+tcp://doge.qubic.li:12480" -u QUBICADDRESS
```

You can also use a **QLI Access Token** instead of your Qubic Address if you have a [pool.qubic.li](https://pool.qubic.li) account.

Optionally pass a rig name: `--rig-id="MySuperRig"`

### Mining Rig Rentals Setup

- **Pool Label:** `Qubic DOGE`
- **Pool Host:Port:** `doge.qubic.li:12480`
- **Workername:** `QUBICADDRESS.workerName` (worker max 12 characters)
- **Password:** *(empty)* or *d=153000000* (difficulty to start the session)

## Transition Plan

The network transitions from XMR to DOGE in 3 phases. [Full details →](https://qubic.org/blog-detail/qubic-dogecoin-mining-transition-plan-april-2026)

| Phase | DOGE | XMR | AI Training | Rewards |
|---|---|---|---|---|
| **1 — Testing** (Apr 1) | ✅ 100% active | 50% | 50% (active when XMR idle) | QUBIC for AI Training and XMR Shares, Bonus for DOGE Shares|
| **2 — Migration** | ✅ 100%, top-up | 50% and less (phasing out) | 50% and more (phasing in, active when XMR idle) | QUBIC for AI Training, XMR and DOGE Shares (pro rata) |
| **3 — Final** | ✅ 100%, top-up | ❌ Removed | ✅ 100% | QUBIC for AI Training (100%) and DOGE (via buyback), no more rewards for XMR |

## Links

- [How the architecture works](https://qubic.org/blog-detail/qubic-dogecoin-mining-how-it-works)
- [Doge Connect (GitHub)](https://github.com/qubic/doge-connect)
- [Discord — #dogecoin channel](https://discord.com/channels/768887649540243497/1406921333635551283)
- [pool.qubic.li](https://pool.qubic.li)
