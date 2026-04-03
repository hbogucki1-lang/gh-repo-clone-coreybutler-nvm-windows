# nvm-windows

> **Windows users:** this repo contains an `install.sh` shell script that is intended for **Linux/macOS only**. Running `source ~/.nvm/nvm.sh` or any other `source` / `.sh` command in Windows PowerShell will **not** work and is not required.
>
> nvm-windows is a **separate native Windows application**. Follow the instructions below.

---

## Installing nvm-windows (Windows)

1. Go to the [Releases page](https://github.com/coreybutler/nvm-windows/releases/latest).
2. Download **`nvm-setup.exe`**.
3. Run the installer **as Administrator** and follow the prompts.
4. **Close and reopen** PowerShell (or Command Prompt) so the updated `PATH` takes effect.

Verify the installation:

```powershell
nvm version
```

### Basic usage

```powershell
# List available Node.js versions
nvm list available

# Install a specific version
nvm install 20

# Switch to that version
nvm use 20

# Confirm
node --version
npm --version
```

> **Note:** You must run PowerShell **as Administrator** when using `nvm install` and `nvm use` on Windows.

---

## install.sh (Linux / macOS only)

The `install.sh` in this repository is the installer for [nvm](https://github.com/nvm-sh/nvm) — the original POSIX shell version of nvm for **Linux and macOS**. It is **not** compatible with Windows PowerShell or Command Prompt.

If you are on Linux or macOS, install nvm with:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.4/install.sh | bash
```

Then load it in your current shell session:

```bash
source ~/.nvm/nvm.sh
```

---

## Further reading

- [nvm-windows GitHub repository](https://github.com/coreybutler/nvm-windows)
- [nvm (Linux/macOS) GitHub repository](https://github.com/nvm-sh/nvm)