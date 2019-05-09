# <em>un</em>common
<img src="screenshot.png" height="508">

_Shown here in [iTerm2](https://www.iterm2.com/) with the [Wombat](https://github.com/djoyner/iTerm2-wombat) color scheme and the [Inconsolata](https://fonts.google.com/specimen/Inconsolata ) typeface._

A fork of the zsh [common](https://github.com/jackharrisonsherlock/common) theme by [Jack Harrison-Sherlock](https://github.com/jackharrisonsherlock).

## Features

### Customizable

Check the `.zsh-theme` file for comments on how to tweak and personalize the theme to your liking.

### Git

Displays current git branch, along with an indicator of the branch's status.

The default symbols are:

- `[•|branch]` - the branch is clean
- `[•|branch,]` - the branch has unstaged changes
- `[•|branch.]` - the branch has staged changes
- `[•|branch;]` - the branch has staged _and_ unstaged changes

### Python Virtualenv

Displays the current `virtualenv` like so: `[my_env|•]` 

### Current working directory

Three options.

1. (Default) Abbreviated [fish](https://github.com/fish-shell/fish-shell)-style paths. `~/Foo/Bar/Baz` → `~/F/B/Baz` 

    **Note**: this requires [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) with the [shrink-path](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/shrink-path) plugin enabled.

2. Deepest directory only. `~/Food/Bar/Baz` -> `Baz`

3. Full path.

### Other stuff!

- Shell symbol changes from `$` to `#` when the user is in privileged mode. (Both symbols are customizable.)
- Displays host when user is SSH'd into another machine. (I don't use this feature much, so it's left entirely intact from the original theme.)

## Installation

### [Oh My Zsh](http://ohmyz.sh) (preferred)

```sh
wget -O $ZSH_CUSTOM/themes/uncommon.zsh-theme https://raw.githubusercontent.com/daturkel/uncommon/master/uncommon.zsh-theme
```

Update your `.zshrc` file with:
```sh
ZSH_THEME="uncommon"
```

### [Antigen](https://github.com/zsh-users/antigen)

Update your `.zshrc` file with:

```sh
antigen bundle daturkel/uncommon
```

### [Antibody](https://github.com/getantibody/antibody)

Update your `.zshrc` file with:

```sh
antibody bundle daturkel/uncommon
```

