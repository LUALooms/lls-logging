# lls-logging
A modular, customizable logging module from LUALooms Studios frameworks.

## ✨ Features
- Fully configurable Discord webhook logging
- Color-coded event types (connect, disconnect, mgmt events, server logs)
- Automatic identifier collection (Steam, Xbox, Discord, License)
- Safe fallback handling for missing identifiers
- Custom per-plugin channels
- Lightweight, optimized,

## 📦 Installation
1. Add the `lls-logging` resource to your `resources` folder.
2. Ensure it's started **before any scripts that depend on it**.
3. Configure your webhook + channels in `config.lua`.

## 🛠 Example Usage
```lua
exports['lls-logging']:sendLog("connect", {
    player = source,
    message = "Player connected to the server"
})
