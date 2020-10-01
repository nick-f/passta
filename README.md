# passta

passta is a highly specific utility to serve a very particular use case.

It is a wrapper for [pass] that provides support for macOS push notifications
when pass performs an action that requires physical interaction with a Yubikey
to decrypt a GPG key stored on it.

Originally this was developed as a helper for [an article I wrote] about using
encrypted environment variables on a local machine for secret and token
storage.

## Installation

1. Download or clone the repo
1. Move the `passta` file to somewhere safe, like `/usr/local/bin`
1. Optional: Add an alias in your shell config (`.bash_profile`, `.zshrc`,
   etc.) to replace the original `pass` with `passta`
   ```
   alias pass='/usr/local/bin/passta'
   ```

## Dependencies

- macOS 10.10 or later
- Ruby (comes pre-installed on macOS)
- [pass]
- [terminal-notifier]

[an article I wrote]: https://www.nickf.dev/encrypted-environment-variables/
[pass]: https://www.passwordstore.org/
[terminal-notifier]: https://github.com/julienXX/terminal-notifier
