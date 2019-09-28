# Introduction to using Terraform Remote Modules

By [Amanda Collins](author contact) and [Erin Atkinson](author contact)

## Goals of this workshop

Understanding of:

* Types of remote modules
* Ways to invoke remote modules
* How to build a remote module
* Architecture considerations for building remote modules

## Prerequisites

* Understanding of Terraform basics
* tfenv/terraform
* Remote Git account (GitHub, GitLab, BitBucket, etc.)

## MacOs

```bash
brew install tfenv
cd workshop
tfenv install
```

## Linux/Windows

Check out tfenv into any path (here is `${HOME}/.tfenv`)

```console
git clone https://github.com/tfutils/tfenv.git ~/.tfenv
```

Add `~/.tfenv/bin` to your `$PATH` any way you like

```console
echo 'export PATH="$HOME/.tfenv/bin:$PATH"' >> ~/.bash_profile
```

OR you can make symlinks for `tfenv/bin/*` scripts into a path that is already added to your `$PATH` (e.g. `/usr/local/bin`) `OSX/Linux Only!`

```console
ln -s ~/.tfenv/bin/* /usr/local/bin
```
  
On Ubuntu/Debian touching `/usr/local/bin` might require sudo access, but you can create `${HOME}/bin` or `${HOME}/.local/bin` and on next login it will get added to the session `$PATH`
or by running `. ${HOME}/.profile` it will get added to the current shell session's `$PATH`.
  
```console
mkdir -p ~/.local/bin/
. ~/.profile
ln -s ~/.tfenv/bin/* ~/.local/bin
which tfenv
```

## Getting started

[Link to rest of workshop](workshop/000_intro.md)
