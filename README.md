# dev-cheat-sheets

Here I note down any information to do with software / computers that I want quick reference to.

I use these cheats sheets in tandem with fzf from my terminal and also within neovim:

From the terminal:

```bash
# this will search my cheet sheets and open them in neovim
tref() {
    if result=($(fd . ${HOME}/tjroot/dev/cheat-sheets | fzf )); then
        nvim $result
    else
        return
    fi
}
```

In neovim: 

```lua
-- this will open cheat sheets in Telescope
cmd("Cs", ":lua require('telescope.builtin').find_files({cwd='~/tjroot/dev/cheat-sheets'})<CR>", {})

```

For oneliner style usage, whereby I want to search for and execute a command directly in the CLI, 
I use [navi](https://github.com/denisidoro/navi).
