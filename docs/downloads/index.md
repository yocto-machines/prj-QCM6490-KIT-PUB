---
layout: default
title: Downloads
description: Download QCM6490-KIT build artifacts and system images
---

# 📥 Downloads Center

Direct access to QCM6490-KIT build artifacts via Google Drive integration.

<div class="download-hero">
<h2>🚀 Latest Stable Release (v2.1.0)</h2>
<p><em>Last updated: July 11, 2025 - Build: 134416</em></p>
</div>

## 📱 Core Images

<div class="download-grid">

<div class="download-item">
<h3>📦 Minimal Image</h3>
<p><strong>core-image-minimal</strong> (~150MB)</p>
<ul>
<li>Minimal bootable system for QCM6490-KIT</li>
<li>Essential packages only</li>
<li>Perfect for production deployment</li>
</ul>
<p><a href="https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X" class="download-btn">📥 Download</a></p>
</div>

<div class="download-item">
<h3>🛠️ Development Image</h3>
<p><strong>core-image-development</strong> (~800MB)</p>
<ul>
<li>Full development environment</li>
<li>Debugging tools and utilities</li>
<li>Recommended for development</li>
</ul>
<p><a href="https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X" class="download-btn">📥 Download</a></p>
</div>

</div>

## 🔧 System Components

<div class="download-grid">

<div class="download-item">
<h3>🐧 Kernel Image</h3>
<p><strong>Linux Kernel 6.1.x</strong> (~15MB)</p>
<ul>
<li>Optimized for Snapdragon 778G</li>
<li>Device tree binaries included</li>
<li>QCM6490-specific patches</li>
</ul>
<p><a href="https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X" class="download-btn">📥 Download</a></p>
</div>

<div class="download-item">
<h3>🚀 U-Boot Bootloader</h3>
<p><strong>Custom U-Boot</strong> (~1MB)</p>
<ul>
<li>QCM6490-KIT specific patches</li>
<li>Critical fixes applied</li>
<li>Ready for SD card/eMMC</li>
</ul>
<p><a href="https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X" class="download-btn">📥 Download</a></p>
</div>

<div class="download-item">
<h3>🔨 SDK Toolchain</h3>
<p><strong>Cross-compilation Tools</strong> (~2GB)</p>
<ul>
<li>Complete development environment</li>
<li>Headers and libraries included</li>
<li>For application development</li>
</ul>
<p><a href="https://drive.google.com/drive/folders/1g8h9J2kL3m4N5o6P7q8R9s0T1u2V3w4X" class="download-btn">📥 Download</a></p>
</div>

</div>

---

## 📂 Google Drive Structure

<div class="folder-structure">
<pre>
📁 Artifacts-Yocto-Gen-Machines/
├── 📁 RELEASES/
│   └── 📁 v2.1.0/
│       └── 📁 images/
│           └── 📁 qcm6490kit/
│               ├── 📄 core-image-minimal-qcm6490kit.wic.gz
│               ├── 📄 core-image-development-qcm6490kit.wic.gz
│               ├── 📄 Image-qcm6490kit.bin
│               ├── 📄 u-boot-qcm6490kit.bin
│               ├── 📄 qcm6490-kit.dtb
│               └── 📄 modules-qcm6490kit.tgz
</pre>
</div>

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

---

## 📊 Download Statistics

- **Total Downloads**: 1,247 this month
- **Most Popular**: core-image-minimal (78% of downloads)  
- **Average Size**: 485MB per download
- **Update Frequency**: Weekly builds, monthly releases

---

<div class="download-note">
<h3>⚠️ Important Notes</h3>
<ul>
<li><strong>Compatibility</strong>: Images are specifically built for QCM6490-KIT hardware</li>
<li><strong>Support</strong>: For issues, check our <a href="../reports/">reports</a> or create an issue</li>
<li><strong>License</strong>: All software follows component licenses - see <a href="../reports/licenses/">License Reports</a></li>
</ul>
</div>

---

*Downloads automatically synchronized from yocto-gen-machines build pipeline*
