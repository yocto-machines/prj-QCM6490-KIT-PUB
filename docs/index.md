---
layout: default
title: QCM6490-KIT Development Hub
---

# 🚀 QCM6490-KIT Development Hub

**Public Documentation Portal** - Migrated from Private Development

Bem-vindo à documentação pública do **Qualcomm QCM6490 Development Kit** usando Yocto Project.

## 🎯 Status do Projeto

<div class="status-section">
    <div class="status-grid">
        <div class="status-item">
            <strong>Board</strong>
            Qualcomm QCM6490 Development Kit
        </div>
        <div class="status-item">
            <strong>Yocto Version</strong>
            Kirkstone (4.0)
        </div>
        <div class="status-item">
            <strong>Repository Type</strong>
            <span class="status-badge status-info">🌍 Public Portal</span>
        </div>
        <div class="status-item">
            <strong>Migration Status</strong>
            <span class="status-badge status-success">✅ Completed</span>
        </div>
    </div>
</div>

## 📋 Documentação Disponível

<div class="quick-links">
    <a href="/reports/" class="quick-link">
        <h3>📊 Build Reports</h3>
        <p>Relatórios de builds, estatísticas e métricas de performance.</p>
    </a>
    
    <a href="/reports/licenses/" class="quick-link">
        <h3>📄 License Compliance</h3>
        <p>Relatórios de conformidade de licenças e análise legal.</p>
    </a>
    
    <a href="/reports/cve/" class="quick-link">
        <h3>🔒 Security Reports</h3>
        <p>Análises de vulnerabilidades CVE e status de segurança.</p>
    </a>
    
    <a href="/downloads/" class="quick-link">
        <h3>⬇️ Downloads</h3>
        <p>Links para artifacts e imagens disponíveis.</p>
    </a>
</div>

## 🏗️ Hub Architecture Migration

Este portal foi **migrado** para a nova arquitetura hub:
🔒 Private Development (/workdir/layers/projects/prj-QCM6490-KIT/)
↓ (migrated to)
🌍 Public Documentation (/workdir/public/prj-QCM6490-KIT-PUB/)
↓ (GitHub Pages)
📱 Public Website

### 🔄 Migration Benefits

- **🔒 Security**: Separation of development and documentation
- **🏗️ Organization**: Hub structure with public/ and layers/
- **📊 Compliance**: Public reports for stakeholders
- **🚀 Scalability**: Template for other machines
- **🔄 Automation**: Continued GitOps integration

## 📊 Quick Start

Para desenvolvedores com acesso ao repositório privado:

```bash
# Build process (unchanged)
cd /workdir
./scripts/enter-qcm6490-build.sh
bitbake core-image-minimal

# Upload and sync (will be updated for new architecture)
./layers/projects/prj-QCM6490-KIT/scripts/machines/qcm6490-kit/qcm6490_upload_script.sh
```

---


Public documentation portal | Hub architecture | Dark Mode 🌙