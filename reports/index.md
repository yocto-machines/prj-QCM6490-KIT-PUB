---
layout: default
title: Reports Overview
---

# 📊 Reports Overview

## Available Report Categories

### 🏗️ [Build Reports](builds/)
- Build status and artifacts
- Performance metrics
- Build configurations

### 📄 [License Reports](licenses/)  
- License compliance analysis
- Package licensing information
- Legal compliance status

### 🔒 [CVE Security Reports](cve/)
- Security vulnerability analysis
- CVE findings and status
- Security compliance metrics

### 📊 [Statistics](statistics/)
- Build performance metrics
- System resource usage
- Hub-level analytics

## 🔄 Auto-Generated Reports

All reports are automatically generated via the Hub-Level GitOps pipeline.

## 📋 Report Categories

{% assign report_types = "builds,licenses,cve,statistics" | split: "," %}
{% for type in report_types %}
### {{ type | capitalize }}
{% assign reports = site.static_files | where_exp: "file", "file.path contains type" %}
{% if reports.size > 0 %}
{% for report in reports limit: 5 %}
- [{{ report.basename }}]({{ report.path }})
{% endfor %}
{% if reports.size > 5 %}
- ... and {{ reports.size | minus: 5 }} more reports
{% endif %}
{% else %}
- No reports available yet
{% endif %}
{% endfor %}

[← Back to Home](../docs/)