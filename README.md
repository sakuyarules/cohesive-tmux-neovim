# Tmux & Neovim Configuration

This is a personal Tmux and Neovim configuration that creates a cohesive and visually appealing terminal experience. The style is inspired by the Catppuccin theme and a desire for a clean, modern, and functional setup.

This configuration is based on the setup discussed in [this GitHub discussion](https://github.com/catppuccin/tmux/discussions/317#discussioncomment-11064512).

## Screenshot

![Screenshot of the Tmux and Neovim setup](Screenshot.png)

## Features

### Tmux

*   **Catppuccin Theme:** The configuration uses the Catppuccin color palette for a consistent look and feel. The colors are defined in `colors.conf`.
*   **Custom Status Bar:** The status bar is customized to show important information at a glance, including:
    *   Session name
    *   Current command
    *   Current path
    *   Zoom status
    *   Memory and CPU usage
    *   Battery percentage
*   **Icon-Based Window Status:** Instead of text, the window status uses icons to represent the current application running in each window (e.g., zsh, nvim, git, etc.).
*   **Custom Keybindings:** The prefix key is set to `` ` `` (backtick) for easier access. Keybindings are set up for intuitive pane navigation, resizing, and window management.
*   **TPM (Tmux Plugin Manager):** The configuration uses TPM to manage Tmux plugins. The following plugins are included:
    *   `tmux-plugins/tpm`
    *   `tmux-plugins/tmux-battery`
    *   `tmux-plugins/tmux-cpu`
    *   `thewtex/tmux-mem-cpu-load`
    *   `laktak/extrakto`

### Neovim (Lualine)

The `lualine.lua` file configures the Lualine plugin for Neovim to match the Tmux theme.

*   **Catppuccin Colors:** The Lualine theme uses the same Catppuccin colors as the Tmux configuration.
*   **Custom Components:** The Lualine status bar is customized to include:
    *   Mode indicator
    *   Git branch
    *   File information (icon, name, and status)
    *   Buffer list
    *   File format, encoding, and size
    *   Diagnostics
    *   Progress and location
*   **Custom Separators:** The status bar uses custom separators for a clean and modern look.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repo-name.git ~/.config/tmux
    ```
2.  **Install TPM (Tmux Plugin Manager):**
    ```bash
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```
3.  **Install the plugins:**
    *   Start Tmux.
    *   Press `prefix` + `I` (capital I, as in **I**nstall) to fetch the plugins.
4.  **Install Neovim and the necessary plugins:**
    *   Install Neovim.
    *   Install a plugin manager for Neovim (e.g., Packer, lazy.nvim).
    *   Add the `nvim-lualine/lualine.nvim` plugin to your Neovim configuration.

## Usage

*   **Reload Tmux configuration:** `prefix` + `r`
*   **Split panes:**
    *   `prefix` + `\` for a horizontal split.
    *   `prefix` + `/` for a vertical split.
*   **Navigate panes:** `prefix` + `h`/`j`/`k`/`l`
*   **Resize panes:** `prefix` + `^h`/`^j`/`^k`/`^l`
*   **Copy mode:** `prefix` + `v`

## Color Palette

The color palette is defined in `colors.conf` and is based on the Catppuccin theme.

| Color Name  | Hex Code  |
| :---------- | :-------- |
| Rosewater   | `#f2d5cf` |
| Flamingo    | `#eebebe` |
| Pink        | `#f4b8e4` |
| Mauve       | `#ca9ee6` |
| Red         | `#e78284` |
| Maroon      | `#ea999c` |
| Peach       | `#ef9f76` |
| Yellow      | `#e5c890` |
| Green       | `#a6d189` |
| Teal        | `#81c8be` |
| Sky         | `#99d1db` |
| Sapphire    | `#85c1dc` |
| Blue        | `#8caaee` |
| Lavender    | `#babbf1` |
| Text        | `#c6d0f5` |
| Subtext1    | `#b5bfe2` |
| Subtext0    | `#a5adce` |
| Overlay2    | `#949cbb` |
| Overlay1    | `#838ba7` |
| Overlay0    | `#737994` |
| Surface2    | `#626880` |
| Surface1    | `#51576d` |
| Surface0    | `#414559` |
| Base        | `#303446` |
| Mantle      | `#292c3c` |
| Crust       | `#232634` |