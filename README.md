# JADX-macOS-Launcher

Installing JADX as a self-contained macOS .app (without contaminating your system with having to install Java):

> Copy from [Ghidra-OSX-Launcher](https://gist.github.com/yifanlu/e9965cdb148b550335e57899f790cad2)

## Build your own

1. Download and extract the launcher AppleScript template app below. Optionally modify `JADX.app/Info.plist` to your liking.
2. You could use custom JADX and JDK version, just put them into `JADX.app/jdk` and `JADX.app/jadx`
3. Or, just `brew install jadx` and `brew install openjdk` then open `JADX.app`

> Note that the template .app is just a standard AppleScript generated .app. If you don't trust the binary, you can build your own with the provided AppleScript and replace `JADX.app/Contents/Resources/Scripts/main.scpt`.
