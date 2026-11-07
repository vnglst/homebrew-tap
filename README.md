# Homebrew tap by vnglst

Install CaptainsLog on Apple Silicon Macs running macOS 26 or later:

```sh
brew install --cask vnglst/tap/captainslog
```

Already installed from `vnglst/captainslog`? Quit CaptainsLog and switch taps:

```sh
brew tap vnglst/tap
brew reinstall --cask --require-sha vnglst/tap/captainslog
brew untap vnglst/captainslog
```

Reinstallation keeps your logs, configuration, and downloaded models.

The cask installs the CaptainsLog app and the `cl` command line tool. The app is ad-hoc signed and not notarized; the cask removes macOS quarantine from the app bundle.

To uninstall the app and move its downloaded models to the Trash while keeping logs and configuration:

```sh
brew uninstall --cask --zap captainslog
```

Empty the Trash to reclaim the model storage. Models in folders you selected yourself are left untouched.

Project source, documentation, and release notes: https://github.com/vnglst/CaptainsLog
