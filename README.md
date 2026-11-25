# Orange Launcher 2

## Windows build

The Windows x64 build is configured in [orange-client-windows.yml](.github/workflows/orange-client-windows.yml).

Upload the prepared source archive named `OrangeClient-source(2)-GitHub.zip` to the repository root. That push starts the build automatically. You can also start it manually from **Actions → Orange Client - Windows EXE → Run workflow** after the archive is present.

The workflow publishes these files as the `Orange-Client-Windows-x64` artifact:
- `Orange-Client-Setup.exe` — Windows installer
- `Orange-Client-Portable.exe` — portable executable
- `SHA256SUMS.txt` — SHA-256 checksums

Builds are unsigned unless a Windows code-signing certificate is configured. Windows SmartScreen may therefore show a warning.
