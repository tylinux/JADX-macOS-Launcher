# JADX-macOS-Launcher

Installing JADX as a self-contained macOS .app (without contaminating your system with having to install Java):

> Copy from [Ghidra-OSX-Launcher](https://gist.github.com/yifanlu/e9965cdb148b550335e57899f790cad2)

## Build your own

1. Download and extract the launcher AppleScript template app below. Optionally modify `JADX.app/Info.plist` to your liking.
2. Download the latest [OpenJDK](http://jdk.java.net/) and extract it to `JADX.app/jdk`, or link exists JDK to here, e.g. `ln -s /Library/Java/JavaVirtualMachines/zulu-15.jdk/ JADX.app/jdk`. Make sure `JADX.app/jdk/Contents/Home/bin/java` exists.
3. Download the latest [JADX](https://github.com/skylot/jadx) and extract it to `JADX.app/jadx`, or link exists JADX to here, e.g. `ln -s /opt/homebrew/Cellar/jadx/1.3.2/ JADX.app/jadx`. Make sure `JADX.app/jadx/bin/jadx-gui` exists.
4. Copy `JADX.app` to your Applications directory.

> Note that the template .app is just a standard AppleScript generated .app. If you don't trust the binary, you can build your own with the provided AppleScript and replace `JADX.app/Contents/Resources/Scripts/main.scpt`.
