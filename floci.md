# fail

```sh
curl -fsSL https://floci.io/install.sh | sh
Installing Floci CLI...
Downloading floci 0.2.1 for darwin-arm64...
Checksum verified.
Installing to /usr/local/bin requires sudo...
Password:
mv: rename /var/folders/r9/smwz67_s3bd15_9m_3x__g3c0000gn/T/tmp.wA118TeYpb to /usr/local/bin/floci: No such file or directory

floci --version
zsh: command not found: floci
```

# wtf

what sort of install process:

* requires sudo
* errs out so pathetically

how badly should I downgrade my expectations of this project?

# goofs

- **Requiring `sudo`** is common for “put binary in `/usr/local/bin`” installers, but it’s not ideal. Better installers offer:

  - user-local install: `~/.local/bin`
  - Homebrew
  - explicit `--prefix`
  - clear manual download instructions

- **Failing because `/usr/local/bin` doesn’t exist** is sloppy. That’s a basic `mkdir -p "$(dirname "$dest")"` miss.
- **The error is especially bad because it downloaded and verified successfully, then failed at the final move.** That suggests the install script got less care than the binary release process.
- **No graceful fallback** / useful message / retry instructions is a negative signal.
