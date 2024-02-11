<!-- panvimdoc-ignore-start -->
# elixir-projectionist.nvim
<!-- panvimdoc-ignore-end -->

# Overview

- [vim-projectionist](https://github.com/tpope/vim-projectionist) elixir support 

This work has been shamelessly copied from [elixir-tools](https://github.com/elixir-tools/elixir-tools.nvim).

I like the feature, but I'm not using the project at this time.

# Install

Requires 0.8

## lazy.nvim

```lua
{
  "smpallen99/elixir-projectionist.nvim",
  config = function()
    require("elixir-projectionist").setup()
  end,
  dependencies = {
    "nvim-lua/plenary.nvim",
  },
}
```
## Suggested Keymap

The following maps `<leader>a` to toggle between the test and source files.

```lua
{
  n = {
    ["<leader>a"] = { "<cmd>A<cr>", "Alternate File", opts = { nowait = true } },
  }
}
```

# Features

### Commands

## Projectionist

[vim-projectionist](https://github.com/tpope/vim-projectionist) integration!

:Esource {args}

: Create or edit a regular source module.

    ```vim
    Esource my_app/accounts/team
    ```

:Etest {args}

: Create or edit a regular test module.

    ```vim
    Etest my_app/accounts/team
    ```

:Etask {args}

: Create or edit a Mix task module.

    ```vim
    Etask server.start
    ```

:Econtroller {args}

: Create or edit a Phoenix controller module.

    ```vim
    Econtroller my_project_web/users
    ```

:Eview {args}

: Create or edit a Phoenix view module.

    ```vim
    Eview my_project_web/users
    ```

:Ehtml {args}

: Create or edit a Phoenix HTML module.

    ```vim
    Ehtml my_project_web/users
    ```

:Ejson {args}

: Create or edit a Phoenix JSON module.

    ```vim
    Ejson my_project_web/users
    ```

:Ecomponent {args}

: Create or edit a Phoenix.Component module.

    ```vim
    Ecomponent my_project_web/users
    ```

:Eliveview {args}

: Create or edit a Phoenix.LiveView module.

    ```vim
    Eliveview my_project_web/users
    ```

:Elivecomponent {args}

: Create or edit a Phoenix.LiveComponent module.

    ```vim
    Elivecomponent my_project_web/users
    ```

:Echannel {args}

: Create or edit a Phoenix channel module.

:Efeature {args}

: Create or edit a Wallaby test module.
