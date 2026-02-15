# Scoop Bucket for KopioRapido

Official [Scoop](https://scoop.sh) bucket for [KopioRapido](https://kopiorapido.com) - a high-performance file copying tool with intelligent transfer optimization.

## Installation

### Quick Install (Both CLI and GUI)
```powershell
scoop bucket add kopiorapido https://github.com/KredoKodo/scoop-kopiorapido
scoop install kopiorapido kopiorapido-gui
```

### CLI Only
```powershell
scoop bucket add kopiorapido https://github.com/KredoKodo/scoop-kopiorapido
scoop install kopiorapido
```

### GUI Only
```powershell
scoop bucket add kopiorapido https://github.com/KredoKodo/scoop-kopiorapido
scoop install kopiorapido-gui
```

## Available Packages

### kopiorapido (CLI)
High-performance command-line file copying tool with:
- Delta sync using FastRsync
- Intelligent transfer engine with automatic strategy selection
- Network transfer compression (Brotli)
- Resume support for interrupted operations
- Multiple operation modes: copy, move, sync, mirror, bidirectional-sync

**Usage:**
```powershell
kopiorapido copy C:\source D:\destination
kopiorapido sync C:\source D:\destination --analyze
kopiorapido --help
```

### kopiorapido-gui (GUI)
Modern desktop application with drag-and-drop interface:
- Visual operation progress with real-time statistics
- Hardware acceleration detection (APFS cloning, ReFS block cloning)
- File integrity verification
- Operation history and resume
- Export performance reports

## Updates

This bucket auto-updates when new KopioRapido releases are published. To update:

```powershell
scoop update
scoop update kopiorapido kopiorapido-gui
```

## Features

- **Intelligent Transfer**: Automatically selects optimal copy strategy based on storage hardware
- **Delta Sync**: Only transfers changed portions of large files
- **Compression**: Transparent compression for network transfers
- **Hardware Acceleration**:
  - Windows: ReFS block cloning, native CopyFile2 API
  - Instant same-volume copies on supported filesystems
- **Resume Support**: Continue interrupted operations
- **Multiple Modes**: Copy, Move, Sync, Mirror, Bidirectional Sync

## Links

- **Website**: https://kopiorapido.com
- **Source Code**: https://github.com/KredoKodo/KopioRapido
- **Documentation**: https://kopiorapido.com/#features
- **Issues**: https://github.com/KredoKodo/KopioRapido/issues

## License

MIT - See [LICENSE](https://github.com/KredoKodo/KopioRapido/blob/main/LICENSE)
