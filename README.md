<div align="center">

<br>

```
    ███╗   ███╗ ██████╗ ███╗   ██╗ ██████╗  ██████╗██╗  ██╗██████╗  ██████╗ ███╗   ███╗███████╗
    ████╗ ████║██╔═══██╗████╗  ██║██╔═══██╗██╔════╝██║  ██║██╔══██╗██╔═══██╗████╗ ████║██╔════╝
    ██╔████╔██║██║   ██║██╔██╗ ██║██║   ██║██║     ███████║██████╔╝██║   ██║██╔████╔██║█████╗  
    ██║╚██╔╝██║██║   ██║██║╚██╗██║██║   ██║██║     ██╔══██║██╔══██╗██║   ██║██║╚██╔╝██║██╔══╝  
    ██║ ╚═╝ ██║╚██████╔╝██║ ╚████║╚██████╔╝╚██████╗██║  ██║██║  ██║╚██████╔╝██║ ╚═╝ ██║███████╗
    ╚═╝     ╚═╝ ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝  ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝ ╚═╝     ╚═╝╚══════╝
```

<br>

![Windows 11](https://img.shields.io/badge/Windows%2011-grey?style=for-the-badge&logo=windows11&logoColor=white)
![License](https://img.shields.io/badge/License-Apache%202.0-grey?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/dhruvin-sarkar/Win11-Rice-Monochrome?style=for-the-badge&color=grey)

<br>

</div>

---

> **Monochrome** is a pure contrast Windows 11 rice

---

## Screenshots

<div align="center">

| Desktop | Terminal |
|:---:|:---:|
| `screenshot here` | `screenshot here` |

| Spotify (Spicetify) | Discord (Vencord) |
|:---:|:---:|
| `screenshot here` | `screenshot here` |

| FlowLauncher | Nilesoft Shell |
|:---:|:---:|
| `screenshot here` | `screenshot here` |

</div>

---

## Software Stack

| Category | Tool |
|---|---|
| **OS** | Windows 11 |
| **Tiling WM** | [Komorebi](https://github.com/LGUG2Z/komorebi) |
| **Status Bar** | [YASB](https://github.com/amnweb/yasb) |
| **Terminal** | Windows Terminal |
| **App Launcher** | [FlowLauncher](https://www.flowlauncher.com/) |
| **Context Menu** | [Nilesoft Shell](https://nilesoft.org/) |
| **Window Tweaks** | [Windhawk](https://windhawk.net/) |
| **Fetch** | [Winfetch](https://github.com/lptstr/winfetch) |
| **Spotify** | [Spicetify](https://spicetify.app/) |
| **Discord** | [Vencord](https://vencord.dev/) |
| **Wallpapers** | Static — included in repo |
| **Font** | [JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads) |

---

## Fonts

Install these before setting anything up — icons and prompt glyphs depend on them.

- **[JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads)** — used everywhere (terminal, YASB, prompt)
- **[JetBrains Mono](https://www.jetbrains.com/lp/mono/)** — non-Nerd variant for editors if preferred

After downloading, right-click the `.ttf` files → **Install for all users**.

---

## Installation

> **Back up your existing configs before copying anything.** All destination paths point to live config locations. If you already use any of these tools, manually merge rather than overwrite.

> Each section shows: `repo folder` → `where to put it on your system`

---

### Komorebi *(Tiling WM)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://youtube.com/@LGUG2Z)

Install Komorebi: [github.com/LGUG2Z/komorebi/releases](https://github.com/LGUG2Z/komorebi/releases)

```
Komorebi/komorebi.json      →  %USERPROFILE%\komorebi.json
Komorebi/komorebi.bar.json  →  %USERPROFILE%\komorebi.bar.json
```

Start with:
```powershell
komorebic start
```

To autostart, add the above command to your PowerShell profile or create a startup script in `shell:startup`.

---

### YASB *(Status Bar)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/results?search_query=yasb+windows+status+bar+setup)

Install: [github.com/amnweb/yasb/releases](https://github.com/amnweb/yasb/releases)

```
YASB/config.yaml  →  %USERPROFILE%\.config\yasb\config.yaml
YASB/styles.css   →  %USERPROFILE%\.config\yasb\styles.css
```

> Requires a Nerd Font for icons to render correctly.

Restart YASB after copying. To autostart, place a shortcut to `yasb.exe` in `shell:startup`.

---

### Windows Terminal

```
Terminal/settings.json  →  %LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState\settings.json
```

Or open Windows Terminal → `Ctrl+Shift+,` to open the settings file directly.

---

### FlowLauncher *(App Launcher)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/results?search_query=flow+launcher+windows+setup+theme)

Install: [flowlauncher.com](https://www.flowlauncher.com/)

```
FlowLauncher/  →  %APPDATA%\FlowLauncher\UserData\
```

> Type `flow user data` inside FlowLauncher to quickly open your UserData folder. Backup and restore by replacing that folder entirely.

---

### Nilesoft Shell *(Context Menu)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/results?search_query=nilesoft+shell+context+menu+windows+11+setup)

Install:
```powershell
winget install -e --id Nilesoft.Shell
```

Or download from [nilesoft.org](https://nilesoft.org/).

```
Nilesoft Shell/shell.nss  →  C:\Program Files\Nilesoft Shell\shell.nss
```

After copying, reload the config with `Ctrl+Right-click` on the desktop.

> You may need to run the file copy as Administrator since it targets `Program Files`. Open an elevated terminal and copy the file manually if needed.

---

### Spicetify

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/watch?v=54y5ZNHIjJw)

Install:
```powershell
iwr -useb https://raw.githubusercontent.com/spicetify/cli/main/install.ps1 | iex
```

```
Spicetify/  →  run: spicetify config-dir  (opens the folder)
```

Copy the theme folder into `Themes/` and the config into the root of the spicetify config dir, then run:

```powershell
spicetify backup apply
```

> After a Spotify update you'll need to re-run `spicetify apply`.

---

### Vencord *(Discord)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/results?search_query=vencord+install+setup+theme+windows)

Install Vencord: [vencord.dev](https://vencord.dev/)

```
Vencord/  →  %APPDATA%\Vencord\themes\
```

After copying the theme `.css` file:

1. Open Discord → Settings → Vencord → **Themes**
2. Under **Local Themes**, click **Open Themes Folder** and confirm the file is there
3. Enable the theme from the list

Alternatively, to use the included CSS as **QuickCSS**:

1. Open Discord → Settings → Vencord → **Themes**
2. Click **Open QuickCSS File**
3. Paste the contents of the `.css` file from the `Vencord/` folder

---

### Windhawk *(Window Tweaks)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-grey?style=flat-square&logo=youtube)](https://www.youtube.com/results?search_query=windhawk+windows+11+taskbar+setup+tutorial)

Install: [windhawk.net](https://windhawk.net/)

```
Windhawk/  →  reference folder — see note below
```

> Windhawk stores mod settings in the Windows registry, not as portable files. The `Windhawk/` folder documents which mods are used and their settings as reference. Install each mod from the Windhawk UI and configure them manually using the values shown.

---

### Winfetch

Install:
```powershell
Install-Script -Name winfetch
```

```
winfetch/config.ps1  →  %USERPROFILE%\.config\winfetch\config.ps1
```

Run with `winfetch` in your terminal.

> If the `.config\winfetch` directory doesn't exist, create it first:
> ```powershell
> mkdir $env:USERPROFILE\.config\winfetch
> ```

---

### Wallpapers

No install needed — the `Wallpapers/` folder contains the static wallpapers used in this rice.

Right-click any image → **Set as desktop background**, or use Windows Settings → Personalization → Background.

---

## Repo Structure

```
Win11-Rice-Monochrome/
├── FlowLauncher/         # App launcher theme + settings
├── Komorebi/             # Tiling WM config
├── Nilesoft Shell/       # Context menu config (shell.nss)
├── Spicetify/            # Spotify theme + config
├── Terminal/             # Windows Terminal settings.json
├── Vencord/              # Discord custom CSS / theme
├── Wallpapers/           # Static monochrome wallpapers
├── Windhawk/             # Windhawk mod settings reference
├── YASB/                 # Status bar config
└── winfetch/             # System fetch config
```

---

## Notes

- **Komorebi without WHKD** — unlike the [Ash rice](https://github.com/dhruvin-sarkar/Win11-Rice-Ash), this setup does not include a WHKD keybinding config. Keybindings are managed elsewhere or not customised.
- **Vencord vs BetterDiscord** — this rice uses Vencord. It's more actively maintained and supports QuickCSS injection directly in settings without needing separate plugin files.
- **Nilesoft Shell admin note** — the config file lives inside `Program Files`, so copying it requires elevated permissions. Run your terminal as Administrator when placing the file.
- **Windhawk settings** — these live in the registry and cannot be portably shared as files. Check the `Windhawk/` folder for the documented settings reference.

---

## Acknowledgements

- [r/unixporn](https://reddit.com/r/unixporn) 
- [LGUG2Z](https://github.com/LGUG2Z) for Komorebi
- [Vencord](https://vencord.dev/) community
- [Spicetify](https://spicetify.app/) community
- [Nilesoft Shell](https://nilesoft.org/) for the context menu

---

<div align="center">

<br>

*if this rice helped you, a ⭐ is appreciated*

<br>

</div>
