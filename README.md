# Orange Launcher 2

## Windows x64 build

The GitHub Actions workflow is `.github/workflows/orange-client-windows.yml`.

It supports either:
- the project directory `OrangeClient/` committed to the repository, or
- `OrangeClient-source(2)-GitHub.zip` in the repository root.

Adding either source layout to `main` starts the build automatically. A manual run is also available under **Actions → Orange Client - Windows EXE → Run workflow**.

The `Orange-Client-Windows-x64` artifact contains:
- `Orange-Client-Setup.exe` — Windows installer
- `Orange-Client-Portable.exe` — portable executable
- `Orange-Client-Portable-Files.zip` — portable executable plus the app-local Microsoft runtime DLLs, when staged
- `SHA256SUMS.txt` — SHA-256 checksums

**Note:** GitHub Actions can only build files committed to this repository. A ZIP attached to a ChatGPT conversation is not automatically available to the GitHub runner. Builds are not Authenticode-signed unless a code-signing certificate is configured, so SmartScreen may show a warning.
