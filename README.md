<p align="center"><img src="https://damnatio.eu/storage/img/banner.png"></p>

<h1 align="center">Damnatio Launcher</h1>


## Features

* 🔒 Full account management.
  * Add multiple accounts and easily switch between them.
  * Microsoft (OAuth 2.0) authentication fully supported.
  * Credentials are never stored and transmitted directly to Mojang.
* 📂 Efficient asset management.
  * Receive client updates as soon as we release them.
  * Files are validated before launch. Corrupt or incorrect files will be redownloaded.
* ☕ **Automatic Java validation.**
  * If you have an incompatible version of Java installed, we'll install the right one *for you*.
  * You do not need to have Java installed to run the launcher.
* 📰 News feed natively built into the launcher.
* ⚙️ Intuitive settings management, including a Java control panel.
* Automatic updates. That's right, the launcher updates itself.

This is not an exhaustive list. Download and install the launcher to gauge all it can do!

## Console

To open the console, use the following keybind.

```console
ctrl + shift + i
```

Ensure that you have the console tab selected. Do not paste anything into the console unless you are 100% sure of what it will do. Pasting the wrong thing can expose sensitive information.

**Build Installers**

To build for your current platform. You first need to install dependencies.

```console
npm install
```

Then ensure `node_modules/helios-core/dist/dl/mojang/MojangIndexProcessor.js` has been updated on line 85-86 like in the <a href="https://github.com/taagada/DamnatioLauncher/blob/master/node_modules/helios-core/dist/dl/mojang/MojangIndexProcessor.js#L85">github</a>.

Then run next command to crate the executable (create the executable depend on the platform your using)

```console
npm run dist
```

Build for a specific platform need to be on the platform.

| Platform    | Command              |
| ----------- | -------------------- |
| Windows x64 | `npm run dist:win`   |
| macOS       | `npm run dist:mac`   |
| Linux x64   | `npm run dist:linux` |
