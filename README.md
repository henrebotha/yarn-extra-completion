# yarn-extra-completion

This plugin is greatly inspired by [zsh-better-npm-completion](https://github.com/lukechilds/zsh-better-npm-completion). It works the same way, as you can see with `npm` demo:

<img src="demo.gif" width="690">

* Makes `yarn add` recommendations from npm cache,
* Makes `yarn remove` recommendations from `dependencies`/`devDependencies`,
* Shows detailed information on script contents for `npm run`,
* Calls already installed yarn completion for any other command.

# Pre-requisites

You'll need [jq](https://stedolan.github.io/jq/download/).

It is strongly suggested that you also have the default yarn suggestion under
the name of `_yarn`. Or that you set `YARN_EXTRA_COMPLETION_DEFAULT=_your_default_function`.

## Installation

### Using [Antigen](https://github.com/zsh-users/antigen)

Bundle `zsh-better-npm-completion` in your `.zshrc`

```shell
antigen bundle buonomo/yarn-completion
```

### Using [zplug](https://github.com/b4b4r07/zplug)
Load `zsh-better-npm-completion` as a plugin in your `.zshrc`

```shell
zplug "buonomo/yarn-completion", defer:2

```
### Using [zgen](https://github.com/tarjoilija/zgen)

Include the load command in your `.zshrc`

```shell
zgen load buonomo/yarn-completion
```

### As an [Oh My ZSH!](https://github.com/robbyrussell/oh-my-zsh) custom plugin

Clone `yarn-completion` into your custom plugins repo

```shell
git clone https://github.com/buonomo/yarn-completion ~/.oh-my-zsh/custom/plugins/yarn-completion
```
Then load as a plugin in your `.zshrc`

```shell
plugins+=(yarn-completion)
```

### Manually
Clone this repository somewhere (`~/.yarn-completion` for example)

```shell
git clone https://github.com/buonomo/yarn-completion.git ~/.yarn-completion
```
Then source it in your `.zshrc`

```shell
source ~/.yarn-completion/yarn-completion.plugin.zsh
```

## License

MIT © Ulysse Buonomo
