# DISPLAZER downloads

DISPLAZER by Dymai Sound is an audio effect for phase dispersion, moving phaser notches, stereo motion, and rhythmic modulation. It includes a studio-rack interface and 37 factory presets.

**[Download the latest Windows release](https://github.com/dejansubotin/displazer-downloads/releases/latest)**

This repository contains public binary downloads and installation information. The development source is maintained separately in a private repository.

## Windows x64

Each release includes:

- `DISPLAZER.vst3`, the complete VST3 plugin folder for a 64-bit Windows DAW.
- `Standalone/DISPLAZER.exe`, an app that runs directly from the extracted folder.
- `INSTALL.txt`, installation instructions.
- A `.sha256` file alongside the ZIP for checking the download.

### Install the VST3

1. Download the ZIP from the release's **Assets** section and extract it completely.
2. Close your DAW.
3. Copy the complete `DISPLAZER.vst3` folder into `C:\Program Files\Common Files\VST3\`. Windows may ask for administrator permission.
4. Restart your 64-bit DAW and rescan VST3 plugins.
5. Find **DISPLAZER** by **Dymai Sound** in the audio effects list.

Keep the `.vst3` folder and all of its contents together.

### Use the standalone app

Open `Standalone/DISPLAZER.exe` from the extracted folder and select your audio device in the app's audio settings. A separate installer is not required.

### Check the download

In PowerShell, run `Get-FileHash .\DISPLAZER-1.1.0-Windows-x64.zip -Algorithm SHA256` and compare the result with the accompanying `.sha256` file. Use the filename for the version you downloaded.

## Validation

Windows releases are compiled using native x64 MSVC on GitHub Actions. Packages are published after the DSP and processor test suites, VST3 validation with pluginval at strictness level 5 (GUI tests skipped), and ZIP integrity checks pass. These automated checks do not cover every DAW or audio device.

## Support

Report problems in this repository's [Issues](https://github.com/dejansubotin/displazer-downloads/issues). Include your Windows version, DAW and version, DISPLAZER version, and steps to reproduce the problem.
