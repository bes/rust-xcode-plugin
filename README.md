# rust-xcode-plugin

This plugin is provided as-is with no guarantees of any kind.

Forked from https://github.com/BrainiumLLC/rust-xcode-plugin

# Modification compared to upstream

* Added support for XCode 15.2.0.

# Update XCode UUID

You can check your UUID with this command:

```shell
$ defaults read /Applications/Xcode.app/Contents/Info DVTPlugInCompatibilityUUID
```

And insert that into `Plug-ins/Rust.ideplugin/Contents/Info.plist`, then update using `setup.sh`,
which will find the currently selected XCode version and install the language support files.
