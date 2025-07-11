---
layout: default
title: QCM6490-KIT Development Hub
---

# 🚀 QCM6490-KIT Development Hub

**Public Documentation Portal** - Migrated from Private Development

Bem-vindo à documentação pública do **Qualcomm QCM6490 Development Kit** usando Yocto Project.

## 🎯 Status do Projeto

| Field | Value |
|-------|-------|
| **Board** | Qualcomm QCM6490 Development Kit |
| **Yocto Version** | Kirkstone (4.0) |
| **Repository Type** | 🌍 Public Portal |
| **Migration Status** | ✅ Completed |

## 📋 Documentação Disponível

### 📊 [Build Reports](../reports/builds/)
Relatórios de builds, estatísticas e métricas de performance.

### 📄 [License Compliance](../reports/licenses/)
Relatórios de conformidade de licenças e análise legal.

### 🔒 [Security Reports](../reports/cve/)
Análises de vulnerabilidades CVE e status de segurança.

### 📊 [Statistics](../reports/statistics/)
Métricas detalhadas de build e performance.

### ⬇️ [Downloads](../downloads/)
Links para artifacts e imagens disponíveis.

## 🏗️ Hub Architecture Migration

Este portal foi **migrado** para a nova arquitetura hub:
🔒 Private Development (/workdir/layers/projects/prj-QCM6490-KIT/)
↓ (migrated to)
🌍 Public Documentation (/workdir/public/prj-QCM6490-KIT-PUB/)
↓ (GitHub Pages)
📱 Public Website

## 🔄 Migration Benefits

* **🔒 Security**: Separation of development and documentation
* **🏗️ Organization**: Hub structure with public/ and layers/
* **📊 Compliance**: Public reports for stakeholders  
* **🚀 Scalability**: Template for other machines
* **🔄 Automation**: Continued GitOps integration

## 📊 Quick Start

Para desenvolvedores com acesso ao repositório privado:

```bash
# Build process (unchanged)
cd /workdir
./scripts/enter-qcm6490-build.sh
bitbake core-image-minimal

# Upload and sync (hub-level)
./scripts/machines/qcm6490-kit/qcm6490_upload_script.sh
```

📋 Latest Reports
Recent Activity

View All Build Reports
View All CVE Reports
View All License Reports
View All Statistics


Public documentation portal - Hub architecture - Dark Mode 🌙