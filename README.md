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

## Licensing and source

This package redistributes official ClamAV binaries, which are licensed under GPL-2.0-only. The NuGet package includes the GPL v2 text, ClamAV's upstream `COPYING.txt`, and the `COPYING/` directory containing notices for bundled third-party components.

The runtime's `SOURCE.txt` identifies its exact upstream binary asset, release, and corresponding source archive. See [Cisco-Talos/clamav releases](https://github.com/Cisco-Talos/clamav/releases) for upstream release materials.
