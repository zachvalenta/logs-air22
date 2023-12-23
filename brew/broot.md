# initial

```sh
$ brew install broot

==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).

==> Downloading https://ghcr.io/v2/homebrew/core/libpthread-stubs/manif
#=#=#                                                                  ######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libpthread-stubs/blobs
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/xorgproto/manifests/20
#=#=#                                                                  ######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/xorgproto/blobs/sha256
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxau/manifests/1.0.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxau/blobs/sha256:c0
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxdmcp/manifests/1.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxdmcp/blobs/sha256:
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxcb/manifests/1.15-
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libxcb/blobs/sha256:0c
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/broot/manifests/1.16.2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/broot/blobs/sha256:eea
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1
######################################################################## 100.0%
==> Installing dependencies for broot: libpthread-stubs, xorgproto, libxau, libxdmcp and libxcb
==> Installing broot dependency: libpthread-stubs
==> Pouring libpthread-stubs--0.4.arm64_monterey.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libpthread-stubs/0.4: 5 files, 6.9KB
==> Installing broot dependency: xorgproto
==> Pouring xorgproto--2022.2.arm64_monterey.bottle.tar.gz
🍺  /opt/homebrew/Cellar/xorgproto/2022.2: 268 files, 3.9MB
==> Installing broot dependency: libxau
==> Pouring libxau--1.0.10.arm64_monterey.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libxau/1.0.10: 20 files, 123KB
==> Installing broot dependency: libxdmcp
==> Pouring libxdmcp--1.1.3.arm64_monterey.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libxdmcp/1.1.3: 11 files, 126KB
==> Installing broot dependency: libxcb
==> Pouring libxcb--1.15.arm64_monterey.bottle.1.tar.gz
🍺  /opt/homebrew/Cellar/libxcb/1.15: 2,461 files, 7.3MB
==> Installing broot
==> Pouring broot--1.16.2.arm64_monterey.bottle.tar.gz
==> Caveats
zsh completions have been installed to:
  /opt/homebrew/share/zsh/site-functions
==> Summary
🍺  /opt/homebrew/Cellar/broot/1.16.2: 15 files, 6.2MB
==> Running `brew cleanup broot`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Caveats
==> broot
zsh completions have been installed to:
  /opt/homebrew/share/zsh/site-functions

$ broot

Broot should be launched using a shell function.
This function most notably makes it possible to cd from inside broot
(see https://dystroy.org/broot/install for explanations).

Can I install it now? [Y/n]
y
Writing br shell function in /Users/zach/Library/Application Support/org.dystroy.broot/launcher/bash/1.
Creating link from /Users/zach/.config/broot/launcher/bash/br to /Users/zach/Library/Application Support/org.dystroy.broot/launcher/bash/1.
/Users/zach/.zshrc successfully patched, you can make the function immediately available with exec zsh

The br function has been successfully installed.
You may have to restart your shell or source your shell init files.
Afterwards, you should start broot with br in order to use its full power.
```

# uninstall

```sh
$ brew uninstall broot

Uninstalling /opt/homebrew/Cellar/broot/1.16.2... (15 files, 6.2MB)

$ brew uninstall -f broot

brew install broot
==> Downloading https://formulae.brew.sh/api/formula.jws.json
######################################################################################################################################## 100.0%
==> Downloading https://formulae.brew.sh/api/cask.jws.json
######################################################################################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/broot/manifests/1.30.2
######################################################################################################################################## 100.0%
==> Fetching broot
==> Downloading https://ghcr.io/v2/homebrew/core/broot/blobs/sha256:23faebec5ff4fd6886a2ec06fc537287b7f5ab9a854816f028d09de761e7eb52
######################################################################################################################################## 100.0%
==> Pouring broot--1.30.2.arm64_monterey.bottle.tar.gz
==> Caveats
zsh completions have been installed to:
  /opt/homebrew/share/zsh/site-functions
==> Summary
🍺  /opt/homebrew/Cellar/broot/1.30.2: 15 files, 8.9MB
==> Running `brew cleanup broot`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).

$ b

Broot's shell function should be upgraded.

Can I proceed? [Y/n]
Y
Removing /Users/zach/.config/broot/launcher/installed-v1.
Removing /Users/zach/Library/Application Support/org.dystroy.broot/launcher/bash/1.
Writing br shell function in /Users/zach/Library/Application Support/org.dystroy.broot/launcher/bash/1.
Removing /Users/zach/.config/broot/launcher/bash/br.
Creating link from /Users/zach/.config/broot/launcher/bash/br to /Users/zach/Library/Application Support/org.dystroy.broot/launcher/bash/1.
/Users/zach/.zshrc already patched, no change made.

The br function has been successfully installed.
You may have to restart your shell or source your shell init files.
Afterwards, you should start broot with br in order to use its full power.
```

# after removing .config/broot

```sh
$ broot
New Configuration files written in "/Users/zach/Library/Application Support/org.dystroy.broot".
You should have a look at them: their comments will help you configure broot.
You should especially set up your favourite editor in verbs.hjson.
```

still doesn't work, even after creating `conf.toml` symlink in `/Users/zach/Library/Application Support/org.dystroy.broot`
