# GitHub Dark Default — bat theme

A [GitHub Dark Default](https://github.com/primer/github-vscode-theme) syntax highlighting theme for [bat](https://github.com/sharkdp/bat) and [delta](https://github.com/dandavison/delta).

## Installation

### bat

```sh
mkdir -p "$(bat --config-dir)/themes"
cp "GitHub Dark Default.tmTheme" "$(bat --config-dir)/themes/"
bat cache --build
```

### delta (lazygit / git pager)

```sh
# ~/.gitconfig or lazygit config
[delta]
    syntax-theme = GitHub Dark Default
```

Or in lazygit `config.yml`:

```yaml
git:
  paging:
    colorArg: always
    pager: delta --dark --paging=never --syntax-theme="GitHub Dark Default"
```

## Preview

![GitHub Dark Default bat theme preview](https://github.com/primer/github-vscode-theme/raw/main/images/dark-default.png)

## License

MIT
