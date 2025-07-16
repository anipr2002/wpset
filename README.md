# wpset

A simple, interactive wallpaper selector for GNOME desktops using `fzf`, `gum`, and `kitty`.

## Description

`wpset` is a command-line tool that allows you to recursively search through a directory of images, navigate through subfolders, preview images directly in the terminal, and set your chosen image as the GNOME desktop background.

## Features

-   Interactive folder navigation using `gum`.
-   Fuzzy-finder based image selection using `fzf`.
-   Image previews directly in the terminal (requires `kitty` terminal).
-   Automatically checks for dependencies and offers to install them.

## Installation

### Arch Linux (via AUR)

You can install `wpset` from the Arch User Repository.
```bash
# Using yay
yay -S wpset

# Using paru
paru -S wpset
```

### Manual Installation

1.  Clone the repository:
    ```bash
    git clone <your-repo-url>
    cd wpset
    ```
2.  Make the script executable:
    ```bash
    chmod +x wpset
    ```
3.  Move the script to a directory in your `$PATH`:
    ```bash
    sudo mv wpset /usr/local/bin/
    ```

## Usage

Simply run the command:
```bash
wpset
```
By default, it will search for images in `~/Pictures`. You can also specify a different directory:
```bash
wpset /path/to/your/images
```

## Dependencies

-   `gum`
-   `fzf`
-   `kitty` (optional, for image previews) 