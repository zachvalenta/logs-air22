# uv itself

```sh
curl -LsSf https://astral.sh/uv/install.sh | sh
downloading uv 0.12.5 aarch64-apple-darwin
installing to /Users/zach/.local/bin
  uv
  uvx
everything's installed!
```

# verify existing Python runtimes

```sh
which python  # /Users/zach/.pyenv/shims/python

uv python list
cpython-3.15.0rc1-macos-aarch64-none                 <download available>
cpython-3.15.0rc1+freethreaded-macos-aarch64-none    <download available>
cpython-3.14.7-macos-aarch64-none                    <download available>
cpython-3.14.7+freethreaded-macos-aarch64-none       <download available>
cpython-3.13.15-macos-aarch64-none                   <download available>
cpython-3.13.15+freethreaded-macos-aarch64-none      <download available>
cpython-3.13.3-macos-aarch64-none                    /opt/homebrew/bin/python3.13 -> ../Cellar/python@3.13/3.13.3/bin/python3.13
cpython-3.13.3-macos-aarch64-none                    /opt/homebrew/bin/python3 -> ../Cellar/python@3.13/3.13.3/bin/python3
cpython-3.12.14-macos-aarch64-none                   <download available>
cpython-3.12.6-macos-aarch64-none                    /opt/homebrew/bin/python3.12 -> ../Cellar/python@3.12/3.12.6/bin/python3.12
cpython-3.11.16-macos-aarch64-none                   <download available>
cpython-3.11.5-macos-aarch64-none                    /opt/homebrew/bin/python3.11 -> ../Cellar/python@3.11/3.11.5/bin/python3.11
cpython-3.10.21-macos-aarch64-none                   <download available>
cpython-3.10.1-macos-aarch64-none                    /Users/zach/.pyenv/shims/python3.10
cpython-3.10.1-macos-aarch64-none                    /Users/zach/.pyenv/shims/python3
cpython-3.10.1-macos-aarch64-none                    /Users/zach/.pyenv/shims/python
cpython-3.9.25-macos-aarch64-none                    <download available>
cpython-3.9.6-macos-aarch64-none                     /usr/bin/python3
cpython-3.8.20-macos-aarch64-none                    <download available>
pypy-3.11.15-macos-aarch64-none                      <download available>
pypy-3.10.16-macos-aarch64-none                      <download available>
pypy-3.9.19-macos-aarch64-none                       <download available>
pypy-3.8.16-macos-aarch64-none                       <download available>

uv run python --version  # Python 3.10.1
uv run python -c "import sys; print(sys.executable)"  # /Users/zach/.pyenv/versions/3.10.1/bin/python
```

# 3.14

```sh
uv python dir  # /Users/zach/.local/share/uv/python
uv python install 3.14  # Installed Python 3.14.7 in 1.73s + cpython-3.14.7-macos-aarch64-none (python3.14)

uv venv --python 3.14
# Using CPython 3.14.7
# Creating virtual environment at: .venv
# Activate with: source .venv/bin/activate

uv run python -c "import ssl, lzma; print('no problems here')"  # no problems here
uv run python --version  # Python 3.14.7
```

# ipython

uv pip install --user --python 3.12 ipython  # error: pip's `--user` is unsupported (use a virtual environment instead)
uv pip install --system --user --python 3.12 ipython  # error: pip's `--user` is unsupported (use a virtual environment instead)

uv tool install --python 3.14 ipython

uv tool install --python 3.14 ipython
Resolved 16 packages in 665ms
Prepared 16 packages in 2.98s
Installed 16 packages in 119ms
 + asttokens==3.0.2
 + executing==2.2.1
 + ipython==9.17.1
 + ipython-pygments-lexers==1.1.1
 + jedi==0.20.0
 + matplotlib-inline==0.2.2
 + parso==0.8.7
 + pexpect==4.9.0
 + prompt-toolkit==3.0.53
 + psutil==7.2.2
 + ptyprocess==0.7.0
 + pure-eval==0.2.4
 + pygments==2.21.0
 + stack-data==0.6.3
 + traitlets==5.16.1
 + wcwidth==0.9.2
Installed 2 executables: ipython, ipython3
