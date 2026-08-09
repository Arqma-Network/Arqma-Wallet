<div align="center">

#  Arqma  Wallet

**A private, secure and untraceable digital currency — you are your own bank.**
Built on CryptoNote technology with ring signatures, stealth addresses and RandomX proof-of-work.

[![Website](https://img.shields.io/badge/WEBSITE-arqma.com-6C3EF4?style=for-the-badge)](https://arqma.com)
[![Discord](https://img.shields.io/badge/DISCORD-Join%20Chat-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://chat.arqma.com)
[![License](https://img.shields.io/badge/LICENSE-BSD--3--Clause-4CAF50?style=for-the-badge)](LICENSE)
[![Release](https://img.shields.io/badge/RELEASE-v10.0.0-2196F3?style=for-the-badge)](https://github.com/arqma/arqma/releases/latest)

</div>

---

## 📥 Downloads — Wallet v5.1.2 / Daemon v10.0.0

<div align="center">

[![Windows](https://img.shields.io/badge/⊞_Download-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](REPLACE_WITH_WINDOWS_LINK)
[![macOS](https://img.shields.io/badge/🍎_Download-macOS-000000?style=for-the-badge&logo=apple&logoColor=white)](REPLACE_WITH_MACOS_LINK)
[![Linux](https://img.shields.io/badge/🐧_Download-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](REPLACE_WITH_LINUX_LINK)

</div>

| Platform | Requirements | File |
|---|---|---|
| 🪟 Windows | Windows 10 or later (64-bit) | `Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe` |
| 🍎 macOS | macOS 11 Big Sur or later (Apple Silicon) | `Arqma-Wallet-Flutter-5.1.2-macos-signed.dmg` |
| 🐧 Linux | Most modern distributions (64-bit) | `Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz` |

Verify every file against the published `SHA256SUMS` on the [Releases page](https://github.com/arqma/arqma/releases/latest).

> Only download from this GitHub Releases page 

---

## 🚀 Install

<details open>
<summary><b>🪟 Windows</b></summary>

1. Download `Arqma-Wallet-Flutter-5.1.2-windows-x64-Setup.exe`
2. Run the installer
3. Launch **Arqma Wallet** from the Start Menu

No extra dependencies needed.
</details>

<details>
<summary><b>🍎 macOS</b></summary>

1. Download the signed `.dmg`, open it, and drag **Arqma Wallet** to Applications
2. Launch from Launchpad

If it won't open (Gatekeeper), run in Terminal:
```bash
xattr -cr "/Applications/Arqma-Wallet.app"
```
</details>

<details>
<summary><b>🐧 Linux</b></summary>

```bash
tar -xzf Arqma-Wallet-Flutter-5.1.2-linux-x64.tar.gz
chmod +x Arqma-Wallet-Flutter-5.1.2-linux-x64.AppImage
./Arqma-Wallet-Flutter-5.1.2-linux-x64.AppImage
```

Pass `--no-sandbox` if the AppImage fails to launch in a restricted environment.
</details>

---

## ✨ Features

- 🔒 Private by default — ring signatures hide sender & amount
- 👤 Untraceable transactions with stealth addresses
- 🔑 25-word mnemonic seed, shown once, for full wallet recovery
- 🔐 Encrypted wallet files
- 🌐 SSL-secured node & wallet connections
- ⚡ Cross-chain atomic swaps
- 🖥️ Cross-platform: Windows, macOS, Linux, Android, iOS
- 🪶 Lightweight, no bundled bloat

---

## 📁 Where things live

| What | Location |
|---|---|
| Blockchain data | `~/.arqma/lmdb/` |
| Wallet files | `~/.arqma/wallets/` |
| Config | `~/.arqma/arqmad.conf` |
| Logs | `~/.arqma/arqmad.log` |

---

## ⚠️ Important

**Your 25-word seed phrase is the only way to recover your funds — write it down and store it offline.** The Arqma team cannot recover lost seed phrases or reverse transactions.

---

## 🛠️ Development

**Prerequisites:** GCC ≥ 7.3, CMake ≥ 3.18, Boost ≥ 1.66, OpenSSL ≥ 1.1.1, libzmq, libsodium

```bash
git clone https://github.com/arqma/arqma
cd arqma && git checkout v10.0.0
git submodule init && git submodule update
```

```bash
make release            # build
make release-test       # optional: run test suite
./bin/arqmad --detach   # run the daemon
```

---

## 📚 Stack

- [CryptoNote](https://cryptonote.org) protocol
- C++ / Boost / OpenSSL / LMDB / ZeroMQ

## 💬 Support

[Discord](https://chat.arqma.com) · [Telegram](https://telegram.arqma.com) · [Matrix](https://matrix.to/#/#arqma:matrix.org) · <support@arqma.com>

## 📄 License

[BSD-3-Clause](LICENSE)
