# ❌ brew

$ brew upgrade node
==> Auto-updating Homebrew...
Adjust how often this is run with `$HOMEBREW_AUTO_UPDATE_SECS` or disable with
`$HOMEBREW_NO_AUTO_UPDATE=1`. Hide these hints with `$HOMEBREW_NO_ENV_HINTS=1` (see `man brew`).
==> Auto-updated Homebrew!
Updated 1 tap (jandedobbeleer/oh-my-posh).

You have 136 outdated formulae and 1 outdated cask installed.

Error: node not installed
==> `brew cleanup` has not been run in the last 30 days, running now...
Disable this behaviour by setting `HOMEBREW_NO_INSTALL_CLEANUP=1`.
Hide these hints with `HOMEBREW_NO_ENV_HINTS=1` (see `man brew`).
Removing: /Users/zach/Library/Caches/Homebrew/portable-ruby-4.0.5_1.arm64_big_sur.bottle.tar.gz... (12.7MB)
Removing: /Users/zach/Library/Caches/Homebrew/Cask/claude-code--2.1.206... (240.4MB)
Removing: /Users/zach/Library/Caches/Homebrew/bootsnap/0ea8e32e2d5779b2ee6b057296a62d6739c9c2dd1ff3a16117c0befbac9d2c64... (1,065 files, 9.7MB)
Removing: /Users/zach/Library/Caches/Homebrew/bootsnap/16e4b77f396cb05f9c9d7cc3db325ed737f1a41f52ffbca011c77ad70f50850b... (1,035 files, 9.2MB)

# ❌ nvm
nvm --version
zsh: command not found: nvm

# ✅ nodenv

 ~  Documents  denv  logs  js  main  ?  which node
/Users/zach/.nodenv/shims/node

 ~  Documents  denv  logs  js  main  ?  nodenv install --list
20.19.2
22.15.1
23.11.1
24.0.2

Only latest stable releases for each Node implementation are shown.
Use 'nodenv install --list-all / -L' to show all local versions.

# ✅ patch so that pi stops crashing on startup
$ nodenv install 22.15.1

To follow progress, use 'tail -f /var/folders/r9/smwz67_s3bd15_9m_3x__g3c0000gn/T/node-build.20260728083811.28833.log' or pass --verbose
Downloading node-v22.15.1-darwin-arm64.tar.gz...
-> https://nodejs.org/dist/v22.15.1/node-v22.15.1-darwin-arm64.tar.gz
Installing node-v22.15.1-darwin-arm64...
Installed node-v22.15.1-darwin-arm64 to /Users/zach/.nodenv/versions/22.15.1

$ nodenv global 22.15.1
$ nodenv rehash
