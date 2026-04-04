# nvm-windows

> **Windows users:** this repo contains an `install.sh` shell script that is intended for **Linux/macOS only**. Running `source ~/.nvm/nvm.sh` or any other `source` / `.sh` command in Windows PowerShell will **not** work and is not required.
>
> nvm-windows is a **separate native Windows application**. Follow the instructions below.

---

## Installing nvm-windows (Windows)

> ⚠️ **Do NOT clone this repository or the nvm-windows source repo to install nvm-windows.**
> Cloning gives you the raw source code, which must be compiled before it can be used.
> You do not need to build anything yourself — use the pre-built installer below.

1. Go to the [Releases page](https://github.com/coreybutler/nvm-windows/releases/latest).
2. Download **`nvm-setup.exe`** (the pre-built Windows installer — not the source code ZIP).
3. Run the installer **as Administrator** and follow the prompts.
4. **Close and reopen** PowerShell (or Command Prompt) so the updated `PATH` takes effect.

Verify the installation:

```powershell
nvm version
```

> **Tip:** If you accidentally cloned the nvm-windows source repository, you can simply delete that folder — it is not needed. Open a **new** PowerShell window after running `nvm-setup.exe` and type `nvm version` to confirm it is installed. To navigate into a folder in PowerShell use `cd <path>`, not the path alone.

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