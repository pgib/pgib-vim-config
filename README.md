# Quick 'n easy Installation

    curl -s https://pgib.me/install/vim | sh

# Neck-beard installation

    cd ~
    git clone https://github.com/pgib/pgib-vim-config.git .vim
    cd .vim
    git submodule update --init
    cd ..
    ln -s .vim/vimrc.conf .vimrc

# Updating

Once you've installed as per above, you can update like so:

```sh
cd ~/.vim
git pull && git submodule update --init
```

# Notable Features

NERDTree activation/deactivation with `,,` (or specifically `<Leader>,`).

![NERDTree](https://cloud.githubusercontent.com/assets/13967/2688572/860d2f86-c2af-11e3-959b-01897cc683af.png)

--------------------

BufExplorer for seeing, managing, and switching between buffers. `<Leader>bb`.

![BufExplorer](https://cloud.githubusercontent.com/assets/13967/2688577/25dda3f6-c2b0-11e3-9fff-f5a4f7bb367f.png)

--------------------

Easily switch between split windows using the `` ` `` (backtick).

![split windows](https://cloud.githubusercontent.com/assets/13967/2688580/a6de7cf0-c2b0-11e3-9d22-e8021a816941.png)

--------------------

Want to make changes to your `~/.vimrc`? Easy: `<Leader>ev`:

![easily edit config](https://cloud.githubusercontent.com/assets/13967/2688583/ef703a08-c2b0-11e3-9582-4993366b0941.png)

Then apply the changes with `<Leader>sv`. (Shout-out to [@flyingoctopus](https://github.com/flyingoctopus/) for this gem.)

--------------------

## Notable Keys

Key-combo    | Description
------------ | -----------
`<Leader>`   | The Vim [Leader key](https://medium.com/usevim/vim-101-what-is-the-leader-key-f2f5c1fa610f) is `,`
`<Leader>c`  | Copy to system clipboard (Mac OS X only)
`<Leader>v`  | Paste from system clipboard (Mac OS X only)
F1           | Line number toggle
F2           | Paste-mode (disables auto intent/comment) toggle
F4           | Close buffer (`:close`)
F5           | Toggle between relative and regular line numbers
Ctrl-n       | Next buffer
Ctrl-p       | Previous buffer
n            | Next match from search and pulse the cursor line
N            | Previous match from search and pulse the cursor line
`<Leader>`cc | Comment the line/selection
`<Leader>`cu | Uncomment the line/selection
Ctrl-w o     | Zoom in and out of the current window
`<Leader>`t  | Search for files *VERY* quickly using fzf
:Rg          | Search within all files *VERY* quickly using ripgrep (must have ripgrep already installed)
