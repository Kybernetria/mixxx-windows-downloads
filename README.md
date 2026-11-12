# Custom Mixxx for Windows x64

Unofficial, unsigned build with SignalSmith, memory cues, and send-only Ableton Link. Not an official Mixxx release.

## Downloads — no GitHub account required

- [Windows installer (.msi)](https://github.com/Kybernetria/mixxx-windows-downloads/releases/download/windows-x64-43164052216/mixxx-1c0b69f-modified-amd64.msi)
- [Portable ZIP](https://github.com/Kybernetria/mixxx-windows-downloads/releases/download/windows-x64-43164052216/Mixxx-protected-Link-Windows-x64-portable.zip)
- [Source and build inputs](https://github.com/Kybernetria/mixxx-windows-downloads/releases/download/windows-x64-43164052216/Mixxx-protected-Link-Windows-x64-source.zip)
- [SHA-256 checksums](https://github.com/Kybernetria/mixxx-windows-downloads/releases/download/windows-x64-43164052216/SHA256SUMS.txt)

Install the [Microsoft Visual C++ v14 x64 Redistributable](https://aka.ms/vc14/vc_redist.x64.exe) first if it is not already installed. These packages do not bundle that runtime. Extract the portable ZIP before running Mixxx.

Windows may show a SmartScreen warning because this custom build is unsigned. Back up your Mixxx settings and library before trying a custom version.

## Verification and limits

Built by CI run `43164052216` from public source `0cwa/mixxx@1c0b69fb1ea1eb4a91c8dd2544efc611b251f3c1` with the supplied source overlay and Windows compatibility patch. Package SHA-256 checksums match the original CI artifact. 175 enabled tests passed; four existing tests were disabled. The local-peer Link protection test and the installed executable's `--version` smoke test passed on the Windows runner.

This is not a clean-machine, real sound-device, or remote Resolume test. The CI runner already has development runtimes installed. A packaging follow-up is investigating bundled runtimes and translations; this release contains the original tested packages, unchanged.

## Source and licenses

The source ZIP includes the complete pinned upstream source snapshot, custom patches, manifest, build scripts, and bundled Link/Asio source archives. `SOURCE-README.md` inside explains the layout and build procedure. The private automation repository and its commit history are not published here.

Mixxx and its dependencies retain their original licenses; see `COPYING`, `LICENSE`, and the notices included with the packages and source. No personal settings or music are included.
