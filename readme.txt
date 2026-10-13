# Pokémon Center Auto Checkout

A Windows-based Pokémon Center checkout automation utility distributed as a standalone executable. The current release includes a Patchright browser setup script, profile directories, and license-key activation.

> **Disclaimer:** This is an independent third-party project and is not affiliated with, endorsed by, or sponsored by The Pokémon Company or Pokémon Center. Use it responsibly and in accordance with applicable website terms and policies. Purchase completion is not guaranteed.

## Features

- **Windows executable:** Run the application using `PokemonBot.exe`.
- **Browser automation environment:** Uses Patchright and its Chromium installation.
- **License activation:** Enter a serial key when prompted.
- **Profile configuration:** Configure a profile before use.

> The public repository currently distributes an executable rather than readable application source code. Internal checkout behavior, supported regions, payment methods, and advanced automation options have not been independently verified.

## Requirements

- Windows
- Python and `pip` available from the command line for installing Patchright
- Internet connection for dependency installation and website access
- A valid serial/license key for application activation

## Installation

1. Download or clone this repository:

   ```bash
   git clone https://github.com/K0126/PokemonCenterAutoCheckout.git
   ```

2. Open the downloaded project folder.
3. Run **`patchright 설치.bat`** to install Patchright and Chromium.

   Alternatively, run these commands manually:

   ```powershell
   pip install patchright
   patchright install chromium
   ```

4. Launch **`PokemonBot.exe`**.
5. Enter your serial key to activate your license.
6. Configure your profile in the application before use.

## Project Structure

```text
PokemonCenterAutoCheckout/
├── PokemonBot.exe         # Windows application
├── patchright 설치.bat    # Patchright + Chromium installer
├── chrome_profile/        # Browser profile directory
├── profiles/              # Application profile directory
└── readme.txt             # Original quick-start instructions
```

## Troubleshooting

**`pip` is not recognized**  
Install Python, enable its PATH integration, reopen your terminal, and retry. You can also try `py -m pip install patchright`.

**Chromium is missing**  
Run `patchright install chromium` again.

**The application does not start**  
Verify that you're on Windows, that the download is complete, and that the browser dependency installation finished successfully.

**License activation fails**  
Double-check the serial key and contact the project maintainer for licensing assistance.

## Security & Privacy

Browser profile folders may contain session cookies, authentication tokens, or other private data. **Do not commit or share populated profiles, credentials, or payment information.** Review the contents of `chrome_profile/` and `profiles/` before publishing or distributing this project. Never enter sensitive information into software you do not trust.
