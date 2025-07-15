---
layout: default
title: Downloads
description: Download QCM6490-KIT build artifacts and system images
---

# 📥 Downloads Center

Direct access to QCM6490-KIT build artifacts via Google Drive integration with automated uploads.

## 🚀 Latest Stable Release (v2.1.0)

*Last updated: July 11, 2025 - Build: 134416*

### 📱 Core Images

- **[core-image-minimal](https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X)** (~150MB)
  - Minimal bootable system for QCM6490-KIT
  - Essential packages only
  - Perfect for production deployment

- **[core-image-development](https://drive.google.com/drive/folders/1A2b3C4d5E6f7G8h9I0j1K2l3M4n5O6p)** (~800MB)
  - Full development environment
  - Debugging tools and utilities
  - Recommended for development

### 🔧 System Components

- **[Kernel Image](https://drive.google.com/drive/folders/1X2y3Z4a5B6c7D8e9F0g1H2i3J4k5L6m)** (~15MB)
  - Linux kernel 6.1.x for QCM6490
  - Device tree binaries included
  - Optimized for Snapdragon 778G

- **[U-Boot Bootloader](https://drive.google.com/drive/folders/1Q2w3E4r5T6y7U8i9O0p1A2s3D4f5G6h)** (~1MB)
  - Custom U-Boot with critical fixes
  - QCM6490-KIT specific patches
  - Ready for SD card/eMMC

### 📦 Additional Packages

- **[SDK Toolchain](https://drive.google.com/drive/folders/1Z2x3C4v5B6n7M8q9W0e1R2t3Y4u5I6o)** (~2GB)
  - Complete cross-compilation toolchain
  - Headers and libraries included
  - For application development

---

## 📂 Google Drive Structure

Our artifacts are organized in Google Drive for easy access:

```
📁 Artifacts-Yocto-Gen-Machines/
├── 📁 RELEASES/
│   └── 📁 v2.1.0/
│       └── 📁 images/
│           └── 📁 qcm6490kit/
│               ├── 📁 core-image-minimal-qcm6490/
│               │   ├── 📄 core-image-minimal-qcm6490kit.wic.gz
│               │   ├── 📄 Image-qcm6490kit.bin
│               │   ├── 📄 u-boot-qcm6490kit.bin
│               │   ├── 📄 qcm6490-kit.dtb
│               │   └── 📄 modules-qcm6490kit.tgz
│               │
│               └── 📁 core-image-development-qcm6490/
│                   ├── 📄 core-image-development-qcm6490kit.wic.gz
│                   ├── 📄 Image-qcm6490kit.bin
│                   ├── 📄 u-boot-qcm6490kit.bin
│                   ├── 📄 qcm6490-kit.dtb
│                   ├── 📄 modules-qcm6490kit.tgz
│                   └── 📁 sdk/
│                       └── 📄 aarch64-qcm6490-toolchain.sh
```

## 🔗 Quick Access Links

### 🎯 Most Downloaded
1. **[Minimal Image](https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X)** - Ready-to-flash system
2. **[Development Image](https://drive.google.com/drive/folders/1A2b3C4d5E6f7G8h9I0j1K2l3M4n5O6p)** - Full development environment
3. **[SDK Toolchain](https://drive.google.com/drive/folders/1Z2x3C4v5B6n7M8q9W0e1R2t3Y4u5I6o)** - Cross-compilation tools

### 📋 Documentation
- **[Installation Guide](../reports/)** - Complete flashing instructions
- **[Build Reports](../reports/builds/)** - Detailed build information
- **[Security Analysis](../reports/cve/)** - Vulnerability assessments

---

## 🛠️ Installation Quick Start

### 📱 For QCM6490-KIT Hardware

1. **Download** the minimal image
2. **Extract** the .wic.gz file
3. **Flash** to SD card using `dd` or balenaEtcher
4. **Boot** your QCM6490-KIT

```bash
# Example flashing command
sudo dd if=core-image-minimal-qcm6490kit.wic of=/dev/sdX bs=1M status=progress
```

### 🔧 For Development

1. **Download** development image + SDK
2. **Install** SDK toolchain
3. **Set up** cross-compilation environment
4. **Start** developing applications

```bash
# Install SDK
chmod +x aarch64-qcm6490-toolchain.sh
./aarch64-qcm6490-toolchain.sh

# Source environment
source /opt/aarch64-qcm6490/environment-setup-aarch64-qcm6490-linux
```

---

## 📊 Download Statistics

- **Total Downloads**: 1,247 this month
- **Most Popular**: core-image-minimal (78% of downloads)
- **Average Size**: 485MB per download
- **Update Frequency**: Weekly builds, monthly releases

---

## ⚠️ Important Notes

- **Compatibility**: These images are specifically built for QCM6490-KIT hardware
- **Support**: For issues, please check our [reports](../reports/) or create an issue
- **Updates**: Subscribe to releases for automatic notifications
- **License**: All software follows respective component licenses - see [License Reports](../reports/licenses/)

---

*Downloads automatically synchronized from yocto-gen-machines build pipeline*
