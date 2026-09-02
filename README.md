[![](https://img.shields.io/nuget/v/soenneker.clamav.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.clamav.windows/)

# Soenneker.Clamav.Windows

The official ClamAV command-line distribution packaged for Windows x64 .NET applications.

```powershell
dotnet add package Soenneker.Clamav.Windows
```

The package copies the ClamAV runtime beneath the application output directory:

```text
Resources/win-x64/clamav/
```

This package contains Windows x64 assets only. Most applications should reference `Soenneker.Clamav.Util`, which selects the correct platform, manages virus definitions, and invokes `clamscan.exe` through a managed API.

The binaries come from the official [Cisco-Talos/clamav releases](https://github.com/Cisco-Talos/clamav/releases) and are distributed under GPL-2.0-only.
