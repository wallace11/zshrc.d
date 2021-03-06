# zshrc.d

> Load ZSH config files from a zshrc.d directory

## Details

Similar to the Fish shell's conf.d directory, this plugin allows you to source your .zshrc configuration from files in a directory.

So, instead of storing all your configuration settings in a single `~/.zshrc` file, you can organize `.zsh` files in a `${ZDOTDIR:-$HOME}/.zshrc.d` directory and this plugin will source all of them.

If using `$ZDOTDIR`, this plugin supports using the non-hidden `$ZDOTDIR/zshrc.d` directory as an alternative.

## Customizing

If you want to use an alternate path, add the following `zstyle` to your `.zshrc` prior to sourcing this plugin:

```zsh
zstyle -s ':zshrc.d:*' 'path' ~/path/to/my/custom/zshrc.d
```

## Installation

Using a Zsh plugin manager:
- [pz]: `pz source mattmc3/zshrc.d`
- [znap]: `znap source mattmc3/zshrc.d`
- [zgenom]: `zgenom load mattmc3/zshrc.d`

Legacy Zsh plugin managers:
- [antibody]: `antibody bundle mattmc3/zshrc.d`
- [zgen]: `zgen load mattmc3/zshrc.d`
- [antigen]: `antigen bundle mattmc3/zshrc.d@main`

[pz]: https://github.com/mattmc3/pz
[antigen]: https://github.com/zsh-users/antigen
[antibody]: https://getantibody.github.io
[znap]: https://github.com/marlonrichert/zsh-snap
[zgen]: https://github.com/tarjoilija/zgen
[zgenom]: https://github.com/jandamm/zgenom
