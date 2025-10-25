# A complete BSPWM Window Manager Environment
<div align = center>

## 👻 Welcome

Welcome to my dotfiles. I’m gh0stzk from Mexico.

These dotfiles are designed with the goal of providing a bspwm environment that is lightweight, efficient, and functional, tailored for any use—whether it’s gaming, web browsing, or a productive work setting.

You’ll have 18 unique themes to choose from, each with its own style, colors, and navigation bar options. With this variety, you’re sure to find one that suits your preferences and needs.

## :book: Wiki
I already started writing the [**Wiki**](https://github.com/gh0stzk/dotfiles/wiki), you should give it a read. If it is your first time with a WM, you may be interested in reading [First steps after installing the dotfiles](https://github.com/gh0stzk/dotfiles/wiki/Firsts-steps-after-installing) or maybe read [frequently asked questions and answers](https://github.com/gh0stzk/dotfiles/wiki/Questions---Answers) [Keybinds](https://github.com/gh0stzk/dotfiles/wiki/Keyboard-Shortcuts) [Firefox Theme](https://github.com/gh0stzk/dotfiles/wiki/Firefox-Theme).

## 🚀 Features
<img src="https://user-images.githubusercontent.com/67278339/221605474-21d65156-0cf7-485c-bd1a-40792c37817e.png" alt="Linux Fetch" align="right" width="450">

#### Change themes on the fly

You can switch themes instantly, with no need to restart your session or environment. With just one click, the change is applied immediately.

#### Consistency Across the Environment

Each theme not only changes the appearance of bspwm but also instantly transforms the color scheme in terminals (Alacritty & Kitty), eww widgets, polybar bars, notifications, gtk theme, launchers and more. Visual harmony is guaranteed in every corner of your system.

#### Performance optimized

BSPWM is not a desktop environment (DE), and that’s exactly what makes it stand out in terms of lightweight performance. On my systems, my BSPWM-dotfiles environment starts with under **500 MB of RAM usage**. While these numbers don't tell the whole story, they do highlight the minimalist approach that a window manager should embrace.

It’s true that Wayland-based environments like Hyprland and Sway are modern and popular, but they come at a cost — for instance, Hyprland typically starts with nearly 1 GB of memory usage, which contradicts the idea of being truly lightweight.

Thanks to the latest major update to Picom, we now have stable and lightweight animations on X11. Additionally, I’ve optimized my setup to avoid unnecessary service reloads. Unlike distributions such as Archcraft or other dotfiles in the web —which restart bspwm, sxhkd, picom, dunst, and others whenever the theme changes— my environment keeps these services running without interruption.

It’s designed so that services/daemons which only need to be launched once do so correctly, and aren’t restarted every time a theme is switched. Changing the theme doesn’t require restarting bspwm, since it’s entirely possible to update its appearance using bspc without reloading the window manager.

In short, my setup is faster, smoother, and more stable than what’s provided by preconfigured distributions.

In addition, each theme can be configured independently — either by manually editing the theme’s configuration file or using my RiceEditor application. This ensures a high level of customization: if you want a minimalist setup for a specific theme, you can disable animations, shadows, rounded borders, or fading effects. On the other hand, if you prefer a more visually rich theme with all those features enabled, that’s fully supported as well. My dotfiles are built to provide that level of flexibility.

#### Multi-Monitor support

If you have multiple monitors, BSPWM will automatically detect and configure up to 4 displays when launching with my dotfiles.

If you connect an additional monitor while the session is already running, simply reload BSPWM using the `Super + Alt + r` key combination, and your monitors will be configured instantly.

You can check the Wiki [👉 Monitors Setup](https://github.com/gh0stzk/dotfiles/wiki/Monitors-setup) if you want to edit the default layouts.

#### RiceEditor

Is an application designed to simplify the customization of your current theme. It allows you to easily adjust various visual and configuration aspects, tailoring your environment to your preferences without the need to manually edit configuration files.

#### Eww Widgets

4 different widgets, including a calendar, music player, profile card and a cheatsheet. These widgets are not only functional but also instantly adapt to the color scheme of the selected theme.

#### Jgmenu

Explore an elegant right-click menu (Desktop) made with Jgmenu, which also syncs with themes for flawless visual consistency. 

#### LockScreen

The lockscreen automatically adapts to the active theme and offers two locking options: it can capture the current screen with a blur effect, or use a specific wallpaper depending on the current theme.

#### Wallpaper Engines

My dotfiles support **5 different methods** for setting your favorite wallpaper:

1. **Theme**: Sets a random wallpaper from the theme’s Walls directory. (Default)
2. **CustomDir**: Sets a random wallpaper from a directory you specify.
3. **CustomImage**: Sets a specific image as wallpaper.
4. **CustomAnimated**: Supports animated wallpapers (.mp4, .mkv, .gif).
5. **Slideshow**: Changes the wallpaper every 15 minutes with a random image from the theme’s Walls directory.

Each option is **theme-specific**, meaning you can have an animated wallpaper in one theme, a static image in another, or a custom directory in a third — And all your settings will be preserved per theme. By default, all themes load a random wallpaper from their Walls folder.

Check the wiki for more details: [👉 Wallpapers Configuration](https://github.com/gh0stzk/dotfiles/wiki/Wallpapers-Configuration)

#### Scratchpad

A _scratchpad_ is a tool designed to provide quick, temporary access to applications or notes without disrupting the desktop workflow. When activated, the scratchpad appears over the current workspace, allowing the user to access applications like a terminal, text editor, or any configured tool. Minimizing it hides the scratchpad from view but keeps it running in the background, ready to be reopened with a simple keyboard shortcut.

It's ideal for quick note-taking, running commands, or accessing auxiliary tools without losing focus on the current task.

#### Visual Composition and Animations

Each theme features a unique color palette, along with transparencies, shadows, and animations—all designed to maintain visual balance without impacting performance or overwhelming the environment.

#### Rofi Applets

Rofi applets to simplify your workflow:

- Wallpaper Selector - See the wiki [WallpaperSelector](https://github.com/gh0stzk/dotfiles/wiki/WallpaperSelector)
- Network Manager
- Bluetooth Controller
- Clipboard Manager
- Screenshot Tool
- Android MTP Manager
- Power Menu
- Keyboard Layout
- Terminal Selector (Alacritty or Kitty)
- Rofi app launcher style selector
- Tab app switcher

#### Tmux Configuration

Benefit from a newly added tmux configuration and design, enhancing your terminal multiplexing experience.

#### Neovim Setup

Simple yet powerful neovim configuration with the following features:

- Treesitter
- Lsp servers
- Completions [blink.nvim](https://github.com/Saghen/blink.nvim)
- Formatting [conform.nvim](https://github.com/stevearc/conform.nvim)
- Picker [Snacks-picker](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md)
- Explorer [Snacks-explorer](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md)
- Tab Line [barbar.nvim](https://github.com/romgrk/barbar.nvim)
- Statusline [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)
- Autopairs [mini-autopairs](https://github.com/echasnovski/mini.nvim/blob/main/readmes/mini-pairs.md)
- Hipatterns [mini-hipatterns](https://github.com/echasnovski/mini.nvim/blob/main/readmes/mini-hipatterns.md)
- Indent guides [Snacks-indent](https://github.com/folke/snacks.nvim/blob/main/docs/indent.md)
- Dashboard [Snacks-dashboard](https://github.com/folke/snacks.nvim/blob/main/docs/dashboard.md)
- WhichKey [which-key.nvim](https://github.com/folke/which-key.nvim)

#### Optimized ZSH Configuration

Optimized, native ZSH configuration. Not __Oh-My-Zsh__ or other bloated plugin managers. Some features:

- Fastest and optimized performance compinit function
- Autocompletion
- Syntax highlighting
- History substring search
- Fzf-tab completion with previews!!

---

> [!CAUTION]
> ⚠️⚠️⚠️ My dotfiles are designed for a **1600x900** resolution with **96 DPI** on a single monitor.
> Some elements may appear different on higher or lower resolutions. You may need to make adjustments to adapt them to your preferences and setup. ⚠️⚠️⚠️

> [!important]
> ✏️✏️✏️ The installer assumes you already have a **functional** Arch Linux installation, whether it’s a fresh install or an existing setup.
>
> A login manager of your choice is required; **lightdm** is recommended.
>
> The rofi connection manager applet, works with **NetworkManager**
>
> If using a virtual machine, be sure to change the Picom backend from **glx** to **xrender** before rebooting, and verify that hardware acceleration is correctly configured in your VM. ✏️✏️✏️

> [!warning]
> :wrench::wrench::wrench: I have tested the installation and functionality of these dotfiles on both high- and low-end machines.
>
> Some adjustments may still be needed, such as changing the Picom backend or VSync settings to ensure compatibility with your graphics card.
>
> If you encounter any issues, feel free to open an [issue](https://github.com/gh0stzk/dotfiles/issues). :wrench::wrench::wrench:

---

### 💾 Installation:

> [!NOTE]
> The installer only works for **ARCH** Linux, and based distros. (Except NO-Systemd ditros like Artix)

Before running this command, check [RiceInstaller](https://raw.githubusercontent.com/gh0stzk/dotfiles/master/RiceInstaller) to make sure it's working and confirm it's safe for your system.

- Open a terminal and execute this commands one by one:

```sh
# Download the installer in your $HOME
curl -LO http://gh0stzk.github.io/dotfiles/RiceInstaller

# Give it execution permission
chmod +x RiceInstaller

# Run the installer
./RiceInstaller
```
