# James Taylor's Dotfiles

Personalized dotfiles managed with [chezmoi](https://www.chezmoi.io/).

## How to Install on a New Machine

1. Install chezmoi:
    ```bash
    sh -c "$(curl -fsLS get.chezmoi.io)"
    ```

2. Initialize and apply dotfiles:
    ```bash
    chezmoi init git@github.com:yourusername/personal-dotfiles.git
    chezmoi apply
    ```

---

## Notes
- Do **not** edit files directly in `~/` — always edit via chezmoi (`chezmoi edit ~/.bashrc`, etc.)
- Sensitive files like `.wakatime.cfg` and `.ssh/` are ignored for security.
- Themes are synced via `~/.themes/`.

---

## Security
- No SSH keys or secret files are included in the repository.
- Always double-check what chezmoi is managing with `chezmoi status`.
  
