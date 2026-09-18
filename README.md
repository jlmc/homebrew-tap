# Homebrew Tap

Homebrew Casks for my macOS applications.

## Installation

First, add the tap:

```bash
brew tap jlmc/tap
````

Then install the desired application using its Cask.

### Rikiki Vault GUI

```bash
brew install --cask rikiki-vault-gui
```

The application will be installed in:

```text
/Applications/rikiki-vault-gui.app
```

## Updating

Update Homebrew and upgrade installed Casks:

```bash
brew update
brew upgrade --cask
```

Or upgrade a specific application:

```bash
brew upgrade --cask rikiki-vault-gui
```

## Uninstalling

To uninstall an application:

```bash
brew uninstall --cask rikiki-vault-gui
```

## Available Casks

| Cask               | Description                |
| ------------------ | -------------------------- |
| `rikiki-vault-gui` | Rikiki Vault GUI for macOS |

## Troubleshooting

If Homebrew reports that the tap or Cask is not trusted, trust the specific Cask:

```bash
brew trust --cask jlmc/tap/rikiki-vault-gui
```

Alternatively, you can trust the entire tap:

```bash
brew trust jlmc/tap
```

> Trusting the entire tap is broader and will also trust future Casks added to this repository.

## Repository Structure

Casks are stored under:

```text
Casks/
├── rikiki-vault-gui.rb
└── ...
```

Each Cask points to a release artifact hosted in the corresponding application's GitHub repository.
