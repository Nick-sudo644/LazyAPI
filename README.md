# 🚀 LazyAPI

**LazyAPI** is a high-performance, server-side Fabric mod designed to eliminate lag spikes caused by massive block updates. Whether it's a 10,000-block TNT explosion or a huge `/fill` command, LazyAPI ensures your game stays fluid.

Optimized specifically with **Apple Silicon M4** performance in mind, but compatible with all modern hardware.

---

## ✨ Features

* **Asynchronous Block Queuing**: Intercepts massive block changes and processes them over multiple ticks.
* **Zero-Lag Explosions**: Enjoy massive craters without the "frozen screen" effect.
* **Chain Reaction Support**: TNT logic remains intact—explosions still trigger nearby TNT and play all sounds/particles.
* **Vanilla Compatible**: Server-side only! Players don't need to install the mod to join your server and benefit from the optimization.
* **High-Speed Processing**: Default limit set to **5,000 blocks per tick**, making full use of high single-core CPU speeds.

---

## 🛠 How it Works

Minecraft usually tries to process all block changes in a single tick. If you break 10,000 blocks at once, the server "hangs" until it's done. 

**LazyAPI** acts as a buffer:
1. It catches the block update requests.
2. It stores them in a safe, concurrent queue.
3. It "feeds" the updates back to the world gradually (but very fast), keeping the frame rate stable and the server responsive.

---

## 📦 Installation & Compatibility

* **Platform**: Fabric
* **Versions**: Minecraft 1.21 to 1.21.11
* **Requirements**: [Fabric API](https://modrinth.com/mod/fabric-api)
* **Side**: Server-side (works in Singleplayer too!)

1. Download the `.jar` from [Modrinth](YOUR_MODRINTH_LINK_HERE).
2. Drop it into your `mods` folder.
3. Launch and enjoy the speed.

---

## 📄 License

This project is licensed under the **Apache License 2.0** - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

* **TheMars** - *Initial Work*

---
*Developed with ❤️ for the Minecraft Community.*
