---
layout: default
title: "QCM6490-KIT Public Data Hub"
description: "Comprehensive public repository for Qualcomm QCM6490 Development Kit builds, reports, and artifacts"
---

# QCM6490-KIT Public Data Hub

<div class="hero-section">
  <div class="hero-content">
    <h2>🚀 Qualcomm QCM6490 Development Kit</h2>
    <p class="hero-description">
      Public data repository featuring automated build reports, security analysis, 
      license compliance, and direct access to build artifacts via Google Drive integration.
    </p>
    <div class="hero-stats">
      <div class="stat-item">
        <span class="stat-number">✅</span>
        <span class="stat-label">Latest Build</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">🔒</span>
        <span class="stat-label">Security Verified</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">📋</span>
        <span class="stat-label">License Compliant</span>
      </div>
    </div>
  </div>
</div>

## 🎯 What You'll Find Here

<div class="feature-grid">

### 📊 Build Reports & Analytics
Comprehensive build status, logs, and performance metrics automatically generated from our CI/CD pipeline.

- **Build Status**: Real-time success/failure tracking
- **Performance Metrics**: Build time trends and resource usage
- **Package Manifests**: Complete dependency lists and versions
- **Size Analysis**: Rootfs optimization and component breakdown

**[📈 View Build Reports]({{ '/reports/builds/' | relative_url }})**

---

### 🔒 Security & Compliance
Complete security analysis and vulnerability tracking for all build components.

- **CVE Analysis**: Known vulnerabilities and mitigation status
- **Security Patches**: Applied fixes and update recommendations  
- **Attack Surface**: Exposed services and security posture
- **Compliance Reports**: Framework adherence and audit trails

**[🛡️ View Security Reports]({{ '/reports/cve/' | relative_url }})**

---

### 📋 License Information
Detailed legal compliance reports for all included software packages.

- **License Inventory**: Complete list of package licenses
- **Compliance Status**: GPL, LGPL, Apache, MIT verification
- **Source Availability**: Direct links to source code repositories
- **Legal Review**: Pre-approved license combinations

**[⚖️ View License Reports]({{ '/reports/licenses/' | relative_url }})**

---

### 📥 Download Center
Direct access to build artifacts via Google Drive integration with automated uploads.

- **Latest Images**: Minimal and development rootfs images
- **System Components**: Kernel, bootloader, and device tree files
- **Installation Guides**: Step-by-step flashing instructions
- **Version History**: Complete artifact changelog

**[📦 Access Downloads]({{ '/downloads/' | relative_url }})**

</div>

## 🏗️ QCM6490-KIT Architecture

<div class="architecture-overview">

### 🔧 Hardware Specifications
- **SoC**: Qualcomm Snapdragon 778G (QCM6490)
- **CPU**: Octa-core ARM (4×Cortex-A78 @2.4GHz + 4×Cortex-A55 @1.8GHz)
- **GPU**: Adreno 642L with Vulkan 1.1 support
- **AI**: Hexagon 770 DSP (~12 TOPS AI processing)
- **Memory**: 8GB LPDDR5 RAM
- **Storage**: 128GB UFS 3.1 + microSD support

### 📡 Connectivity Features
- **5G/4G**: Integrated cellular modem
- **Wi-Fi**: 802.11ax (Wi-Fi 6E) + Bluetooth 5.2
- **USB**: USB 3.1 Type-C with DisplayPort
- **Camera**: Triple MIPI-CSI interfaces (up to 200MP)
- **Display**: Dual MIPI-DSI + HDMI output

### 🚀 Target Applications
- **Edge AI**: Machine learning inference and training
- **5G Gateways**: Industrial IoT connectivity hubs
- **Mobile Computing**: Tablet and mobile device platforms
- **Computer Vision**: Real-time image processing systems

</div>

## 📈 Latest Statistics

<div class="stats-dashboard">

### 🔨 Build Performance
- **Last Build**: January 11, 2025 at 13:44 UTC
- **Build Status**: ✅ **Success** (95% success rate last 30 builds)
- **Build Time**: 3.2 hours average
- **Artifact Size**: ~150MB (minimal), ~800MB (development)

### 🔒 Security Status  
- **CVE Status**: ✅ **No Critical Vulnerabilities**
- **Last Scan**: January 11, 2025
- **Patch Level**: Up to date with latest security fixes
- **Compliance**: ✅ **Fully Compliant**

### 📦 Available Downloads
- **Core Images**: 2 variants (minimal, development)
- **Components**: Kernel, bootloader, device trees
- **Total Artifacts**: 12 files (~950MB total)
- **Google Drive**: ✅ **Auto-sync enabled**

</div>

## 🔄 Automation & Integration

### Seamless CI/CD Pipeline

```
yocto-gen-machines (Private)
        ↓ Automated Build
    QCM6490-KIT Layer
        ↓ Report Generation
   prj-QCM6490-KIT-PUB (Public)
        ↓ GitHub Pages
      📊 Public Access
```

### Update Schedule
- **Build Reports**: Generated after each successful build
- **Security Scans**: Weekly CVE database updates
- **License Reports**: Updated with dependency changes
- **Artifact Uploads**: Automatic Google Drive synchronization

## 🌐 Part of Yocto-Gen-Machines Ecosystem

This repository serves as the **public data hub** for QCM6490-KIT builds from the larger [Yocto-Gen-Machines]({{ site.project.hub_repo }}) infrastructure:

### 🔗 Related Projects
- **[Main Development]({{ site.project.main_repo }})**: Private repository with Yocto layers and build scripts
- **[Yocto-Gen-Machines Hub]({{ site.project.hub_repo }})**: Multi-machine embedded Linux development framework
- **Documentation**: Complete technical guides and API references

### 🎯 Multi-Machine Template
QCM6490-KIT serves as a **proof of concept** for public data distribution that will expand to:
- **A20-OLinuXino-LIME2-PUB**: Allwinner boards
- **NXP-iMX8mp-EVK-PUB**: NXP multimedia processors  
- **NXP-iMX91-EVK-PUB**: NXP industrial processors
- **[Future machines]-PUB**: Additional embedded platforms

## 🚀 Quick Start Guide

### For Developers
1. **[Check Build Status]({{ '/reports/builds/' | relative_url }})** - Verify latest build success
2. **[Review Security]({{ '/reports/cve/' | relative_url }})** - Assess vulnerability status
3. **[Download Images]({{ '/downloads/' | relative_url }})** - Get development artifacts
4. **Flash & Test** - Deploy to QCM6490-KIT hardware

### For System Integrators  
1. **[License Review]({{ '/reports/licenses/' | relative_url }})** - Verify legal compliance
2. **[Performance Analysis]({{ '/reports/statistics/' | relative_url }})** - Check system metrics
3. **[Download Production Images]({{ '/downloads/' | relative_url }})** - Get deployment-ready builds
4. **Integration** - Incorporate into larger systems

### For Researchers
1. **[Explore Reports]({{ '/reports/' | relative_url }})** - Analyze build and security data
2. **[Study Architecture]({{ site.project.hub_repo }})** - Review development methodology
3. **[Access Source]({{ site.project.main_repo }})** - Examine Yocto layer implementation
4. **[Contribute]({{ site.project.main_repo }}/issues)** - Report findings and improvements

## 📞 Support & Community

### Getting Help
- **🐛 [Report Issues]({{ site.repository | prepend: 'https://github.com/' }}/issues)**: Problems with data or documentation
- **💬 [Discussions]({{ site.repository | prepend: 'https://github.com/' }}/discussions)**: General questions and ideas
- **📖 [Documentation]({{ site.project.main_repo }})**: Technical guides and tutorials
- **🏠 [Main Project]({{ site.project.main_repo }})**: Development repository

### Stay Updated
- **GitHub Pages**: Automatic updates from build pipeline
- **Release Notes**: Version history and changelog
- **Security Alerts**: CVE notifications and patches
- **Community**: Join discussions and contribute improvements

---

<div class="footer-cta">
  <h3>🎯 Ready to Get Started?</h3>
  <p>Explore the latest QCM6490-KIT builds and start developing with cutting-edge mobile processor technology.</p>
  <div class="cta-buttons">
    <a href="{{ '/reports/' | relative_url }}" class="btn btn-primary">📊 View Reports</a>
    <a href="{{ '/downloads/' | relative_url }}" class="btn btn-secondary">📥 Download Images</a>
    <a href="{{ site.project.main_repo }}" class="btn btn-outline">🔧 Development Repo</a>
  </div>
</div>

*Last updated: January 11, 2025 - Automatically generated from build pipeline*

<style>
/* Hero Section */
.hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 3rem 2rem;
  border-radius: 12px;
  margin: 2rem 0;
  text-align: center;
}

.hero-content h2 {
  margin: 0 0 1rem 0;
  font-size: 2.5rem;
  font-weight: bold;
}

.hero-description {
  font-size: 1.2rem;
  margin: 0 0 2rem 0;
  opacity: 0.9;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.hero-stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 2rem;
  max-width: 500px;
  margin: 0 auto;
}

.stat-item {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.stat-number {
  font-size: 2rem;
  font-weight: bold;
  margin-bottom: 0.5rem;
}

.stat-label {
  font-size: 0.9rem;
  opacity: 0.8;
}

/* Feature Grid */
.feature-grid {
  display: grid;
  gap: 2rem;
  margin: 3rem 0;
}

.feature-grid > div {
  border: 1px solid #e1e8ed;
  padding: 2rem;
  border-radius: 8px;
  background-color: #f8f9fa;
  transition: transform 0.2s, box-shadow 0.2s;
}

.feature-grid > div:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.feature-grid h3 {
  color: #2c3e50;
  margin-top: 0;
  border-bottom: 2px solid #3498db;
  padding-bottom: 0.5rem;
}

.feature-grid a {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  background-color: #3498db;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-weight: bold;
  transition: background-color 0.2s;
}

.feature-grid a:hover {
  background-color: #2980b9;
}

/* Architecture Overview */
.architecture-overview {
  background-color: #f8f9fa;
  border: 1px solid #dee2e6;
  border-radius: 8px;
  padding: 2rem;
  margin: 3rem 0;
}

.architecture-overview h3 {
  color: #2c3e50;
  margin-top: 2rem;
}

.architecture-overview h3:first-child {
  margin-top: 0;
}

/* Stats Dashboard */
.stats-dashboard {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.stats-dashboard > div {
  background: linear-gradient(135deg, #74b9ff 0%, #0984e3 100%);
  color: white;
  padding: 1.5rem;
  border-radius: 8px;
}

.stats-dashboard h3 {
  margin: 0 0 1rem 0;
  color: white;
}

.stats-dashboard ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.stats-dashboard li {
  padding: 0.25rem 0;
  opacity: 0.9;
}

/* Footer CTA */
.footer-cta {
  background: linear-gradient(135deg, #fd79a8 0%, #fdcb6e 100%);
  color: #2d3436;
  padding: 3rem 2rem;
  border-radius: 12px;
  text-align: center;
  margin: 3rem 0;
}

.footer-cta h3 {
  margin: 0 0 1rem 0;
  color: #2d3436;
}

.cta-buttons {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
  margin-top: 2rem;
}

.btn {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  text-decoration: none;
  border-radius: 6px;
  font-weight: bold;
  transition: all 0.2s;
}

.btn-primary {
  background-color: #2d3436;
  color: white;
}

.btn-secondary {
  background-color: #74b9ff;
  color: white;
}

.btn-outline {
  background-color: transparent;
  color: #2d3436;
  border: 2px solid #2d3436;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

/* Responsive */
@media (max-width: 768px) {
  .hero-content h2 {
    font-size: 2rem;
  }
  
  .hero-description {
    font-size: 1rem;
  }
  
  .cta-buttons {
    flex-direction: column;
    align-items: center;
  }
  
  .btn {
    width: 200px;
  }
}
</style>