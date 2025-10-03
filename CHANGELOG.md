# Change Log

## [0.1.1] - 2025-10-03

### Added
- 📱 **Run with Emulator** - Fitur baru untuk menjalankan URL di Android Emulator atau iOS Simulator
  - Auto-detect ketersediaan Android SDK dan iOS Simulator
  - Smart platform selection (otomatis pilih jika hanya 1 platform tersedia)
  - List dan pilih emulator/simulator yang sudah berjalan
  - Start emulator baru jika belum ada yang berjalan
  - List dan pilih Android AVD yang tersedia untuk di-start
  - List dan pilih iOS Simulator yang tersedia untuk di-start
  - Auto-open URL di emulator setelah boot selesai
  - Tombol otomatis tersembunyi jika tidak ada platform yang tersedia
- ⌨️ **Keyboard Shortcuts**:
  - `Ctrl+Alt+E` / `Cmd+Option+E` untuk Run with Emulator
    - Shortcut global - bisa dijalankan dari mana pun (tidak perlu buka Device Simulator dulu)
    - Langsung start fresh emulator tanpa URL
    - Pilih platform dan device yang ingin dijalankan
  - `Ctrl+M` / `Cmd+M` sekarang menampilkan quick picker:
    - Web Device Simulator (simulator web-based)
    - Android Emulator (langsung ke pilihan AVD)
    - iOS Simulator (langsung ke pilihan simulator)
- 🎯 **Toolbar Icon**: Icon mobile (📱) ditambahkan di editor toolbar (navigation group)
  - Klik icon untuk menampilkan quick picker yang sama dengan `Ctrl+M`
  - Posisi di samping icon split editor
  - Akses cepat tanpa keyboard shortcut
- 🎨 **UI Improvements**:
  - Tombol "Run with Emulator" dengan styling konsisten seperti device selector
  - Layout responsive dengan flex-wrap untuk layar kecil

### Changed
- 🏗️ **Code Refactoring**:
  - Separation of concerns antara UI dan business logic
- 📐 **Layout Optimization**:
  - Better spacing dan alignment untuk toolbar
  - Responsive breakpoints untuk berbagai ukuran layar

## [0.1.0] - 2025-10-01

### Added
- Initial release of Device Simulator
- Device dropdown dengan 15+ preset devices:
  - iPhone (13 Pro, 15, 15 Pro Max, 12 Mini, 14 Pro, 11)
  - iPad (Pro 11, Air, Mini)
  - Android (Samsung Galaxy S25, Google Pixel 9, OnePlus 10 Pro, Xiaomi 14, Galaxy Tab S8, Pixel Tablet)
- Custom viewport sizes
- Rotate viewport functionality
- Manual resize with drag handles
- Zoom controls (10%-200%)
  - Zoom in/out buttons
  - Reset zoom to 100%
  - Fit to screen functionality
- URL input for loading websites
- Live preview in VSCode
- Smart reload - tetap di halaman yang sama saat ganti device
- Keyboard shortcut (Ctrl+Shift+V / Cmd+Shift+V)
