---
layout: default
title: "Download Center"
description: "Access QCM6490-KIT build artifacts, images, and documentation via Google Drive integration"
---

# Download Center 

Access the latest QCM6490-KIT build artifacts including rootfs images, kernel files, and development tools.

## 🚀 Quick Downloads

### Latest Stable Release (v2.1.0)

<div class="download-grid">

#### 📱 Core Images
- **[core-image-minimal](https://drive.google.com/drive/folders/artifacts-folder-id)** (~150MB)
  - Minimal bootable system for QCM6490-KIT
  - Essential packages only
  - Perfect for production deployment

- **[core-image-development](https://drive.google.com/drive/folders/artifacts-folder-id)** (~800MB)
  - Full development environment
  - Debugging tools and utilities
  - Recommended for development

#### 🔧 System Components
- **[Kernel Image](https://drive.google.com/drive/folders/kernel-folder-id)** (~15MB)
  - Linux kernel 6.1.x for QCM6490
  - Device tree binaries included
  - Optimized for Snapdragon 778G

- **[U-Boot Bootloader](https://drive.google.com/drive/folders/uboot-folder-id)** (~1MB)
  - Custom U-Boot with critical fixes
  - QCM6490-KIT specific patches
  - Ready for SD card/eMMC

</div>

## 📂 Google Drive Structure

Our artifacts are organized in Google Drive for easy access:

```
Artifacts-Yocto-Gen-Machines/
└── RELEASES/
    └── v2.1.0/
        └── images/
            └── qcm6490kit/
                ├── core-image-minimal-qcm6490/
                │   ├── images/          # 5 rootfs files
                │   ├── kernel/          # 2 kernel files
                │   └── manifest.json    # Build metadata
                └── core-image-development/
                    ├── images/
                    ├── kernel/
                    └── manifest.json
```

## 🔗 Direct Access Links

### 📥 Main Artifact Folder
**[🗂️ QCM6490-KIT Artifacts](https://drive.google.com/drive/folders/1ABC123-your-folder-id)**
- All build artifacts organized by version
- Automatic uploads from CI/CD pipeline
- Includes metadata and manifests

### 📊 Build Reports
**[📋 Latest Build Reports](../reports/builds/)**
- Detailed build logs and status
- Package manifests and dependencies
- Build performance metrics

### 🔒 Security Information
**[🛡️ Security Reports](../reports/cve/)**
- CVE analysis and vulnerability status
- Security patches information
- Compliance reports

## 💾 Installation Instructions

### SD Card Flashing (Recommended)

```bash
# Download the image
wget [Google Drive direct link to .wic file]

# Flash to SD card (replace /dev/sdX with your SD card)
sudo dd if=core-image-minimal-qcm6490-kit.rootfs.wic \
        of=/dev/sdX \
        bs=4M \
        status=progress \
        conv=fsync

# Safely eject
sudo eject /dev/sdX
```

### eMMC Flashing (Advanced)

```bash
# Using fastboot (QCM6490-KIT in fastboot mode)
fastboot flash system core-image-minimal-qcm6490-kit.rootfs.ext4

# Or using custom flashing tools
# See documentation for board-specific instructions
```

## 🔍 File Types Available

| File Type | Extension | Description | Use Case |
|-----------|-----------|-------------|----------|
| **Root Filesystem** | `.rootfs.ext4` | Complete Linux filesystem | SD card/eMMC flashing |
| **WIC Image** | `.rootfs.wic` | Complete disk image | Direct SD card writing |
| **Compressed Archive** | `.rootfs.tar.gz` | Filesystem archive | Custom deployment |
| **Kernel Image** | `Image` | Linux kernel binary | Boot partition |
| **Device Tree** | `.dtb` | Hardware description | Boot configuration |
| **Modules** | `.tgz` | Kernel modules | Runtime loading |

## 📋 Build Metadata

Each build includes comprehensive metadata:

### Build Information
- **Build Date**: Timestamp of compilation
- **Git Commit**: Exact source code version
- **Build Host**: Environment details
- **Build Time**: Duration and performance

### Package Manifest
- **Installed Packages**: Complete list with versions
- **Dependencies**: Package dependency tree
- **Licenses**: Legal compliance information
- **Security**: CVE status for all packages

### Quality Metrics
- **Size Analysis**: Rootfs and component sizes
- **Performance**: Boot time and resource usage
- **Test Results**: Automated validation status

## 🔄 Version History

| Version | Date | Size | Notes |
|---------|------|------|-------|
| **v2.1.0** | 2025-01-11 | ~150MB | Latest stable with Google Drive integration |
| v2.0.0 | 2025-01-06 | ~140MB | Initial QCM6490-KIT support |
| v1.9.0 | 2024-12-20 | ~135MB | Beta release with critical fixes |

### 📈 What's New in v2.1.0
- ✅ **Smart upload system** with automated Google Drive distribution
- ✅ **Critical U-Boot fixes** for circular dependency issues
- ✅ **Improved stability** with sequential build strategy
- ✅ **Enhanced metadata** with detailed manifests
- ✅ **Security updates** with latest CVE patches

## 🔧 Development Downloads

### Source Code Access
- **[Main Project Repository](https://github.com/yocto-machines/prj-QCM6490-KIT)**
- **[Yocto-Gen-Machines Hub](https://github.com/yocto-machines/yocto-gen-machines)**
- **[Layer Source Code](https://github.com/yocto-machines/prj-QCM6490-KIT/tree/main/recipes-core)**

### Development Tools
- **Build Environment**: Docker container with all dependencies
- **CI/CD Scripts**: Automated build and test pipeline
- **Documentation**: Technical guides and API references

## 📞 Support & Troubleshooting

### Common Issues

**Q: Download is slow or fails**
- A: Try using Google Drive's direct download feature
- Check your internet connection stability
- Use download managers for large files

**Q: Image doesn't boot on hardware**
- A: Verify SD card integrity with `fsck`
- Check if you're using the correct image for your board revision
- Ensure proper power supply (5V/3A recommended)

**Q: Missing files in download**
- A: Check the build date - some components may not be included in minimal images
- Use development image for complete toolset
- Review build manifest for package list

### Getting Help
- **[GitHub Issues](https://github.com/yocto-machines/prj-QCM6490-KIT-PUB/issues)**: Report problems or request features
- **[Build Reports](../reports/builds/)**: Check if issue is known
- **[Main Project](https://github.com/yocto-machines/prj-QCM6490-KIT)**: Development discussions

## 🔐 Security & Verification

### File Integrity
All downloads include checksums for verification:

```bash
# Verify download integrity
sha256sum core-image-minimal-qcm6490-kit.rootfs.wic
# Compare with published checksum in manifest.json
```

### Security Scanning
- **CVE Analysis**: All packages scanned for known vulnerabilities
- **License Compliance**: Legal review completed
- **Supply Chain**: Source code authenticity verified

---

*Downloads automatically updated from CI/CD pipeline. Last update: 2025-01-11 13:44 UTC*

<style>
.download-grid {
    display: grid;
    gap: 1.5rem;
    margin: 2rem 0;
}

.download-grid > div {
    border: 1px solid #3498db;
    padding: 1.5rem;
    border-radius: 8px;
    background-color: #f8f9fa;
}

.download-grid h4 {
    color: #2c3e50;
    margin-top: 0;
    border-bottom: 2px solid #3498db;
    padding-bottom: 0.5rem;
}

.download-grid ul {
    list-style: none;
    padding: 0;
}

.download-grid li {
    margin: 1rem 0;
    padding: 0.75rem;
    background-color: white;
    border-radius: 4px;
    border-left: 4px solid #3498db;
}

.download-grid a {
    font-weight: bold;
    color: #2980b9;
    text-decoration: none;
}

.download-grid a:hover {
    text-decoration: underline;
}

table {
    width: 100%;
    border-collapse: collapse;
    margin: 1.5rem 0;
}

table th, table td {
    border: 1px solid #ddd;
    padding: 0.75rem;
    text-align: left;
}

table th {
    background-color: #3498db; 
    color: white;
    font-weight: bold;
}

table tr:nth-child(even) {
    background-color: #f2f2f2;
}

.version-latest {
    background-color: #e8f5e8 !important;
    font-weight: bold;
}

code {
    background-color: #f4f4f4;
    padding: 0.2rem 0.4rem;
    border-radius: 3px;
    font-family: 'Courier New', monospace;
}

pre {
    background-color: #2c3e50;
    color: #ecf0f1;
    padding: 1rem;
    border-radius: 6px;
    overflow-x: auto;
}

.file-structure {
    background-color: #f8f9fa;
    border: 1px solid #dee2e6;
    border-radius: 6px;
    padding: 1rem;
    font-family: 'Courier New', monospace;
    font-size: 0.9rem;
}
</style>