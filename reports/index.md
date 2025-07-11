---
layout: default
title: "Reports Dashboard"
description: "Comprehensive reports for QCM6490-KIT builds including security, licensing, and performance data"
---

# Reports Dashboard

Welcome to the QCM6490-KIT reports center. Here you'll find comprehensive information about builds, security, licensing, and performance metrics.

## 📊 Report Categories

<div class="report-grid">

### 🔨 Build Reports
**Latest build status and detailed logs**
- Build success/failure status
- Compilation logs and error analysis
- Package manifests and dependency trees
- Build artifacts and size analysis

[📁 View Build Reports](./builds/) | [📄 Latest Build](./builds/latest.html)

---

### 🔒 Security Reports  
**CVE analysis and vulnerability tracking**
- Known vulnerabilities assessment
- Security patches and updates
- Attack surface analysis
- Compliance status reports

[🛡️ View Security Reports](./cve/) | [🔍 Latest CVE Analysis](./cve/latest.html)

---

### 📋 License Reports
**Legal compliance and license information**
- Complete license inventory
- GPL/LGPL/Apache/MIT compliance
- Source code availability
- Legal review summaries

[⚖️ View License Reports](./licenses/) | [📜 Latest License Report](./licenses/latest.html)

---

### 📈 Performance Statistics
**Build metrics and performance trends**
- Build time trends
- Resource usage analysis
- Artifact size tracking
- Success rate metrics

[📊 View Statistics](./statistics/) | [📈 Latest Stats](./statistics/latest.html)

</div>

## 🕒 Recent Activity

### Latest Reports Generated
{% assign latest_date = "2025-01-11" %}

| Report Type | Last Updated | Status | Quick Link |
|-------------|--------------|--------|------------|
| 🔨 Build | {{ latest_date }} 13:44 | ✅ Success | [View](./builds/build-20250711-134416.html) |
| 🔒 CVE | {{ latest_date }} 13:44 | ✅ Clean | [View](./cve/cve-20250711-134416.html) |
| 📋 License | {{ latest_date }} 13:44 | ✅ Compliant | [View](./licenses/licenses-20250711-134416.html) |
| 📈 Stats | {{ latest_date }} 13:44 | ✅ Updated | [View](./statistics/stats-20250711-134416.html) |

## 🔄 Auto-Generated Reports

All reports in this section are **automatically generated** by the CI/CD pipeline from the main [prj-QCM6490-KIT]({{ site.project.main_repo }}) repository.

### Update Schedule
- **Build Reports**: Generated after each successful build
- **Security Reports**: Updated weekly with latest CVE database
- **License Reports**: Updated when package dependencies change
- **Statistics**: Aggregated daily from build metrics

### Report Format
Each report includes:
- **Timestamp**: When the report was generated
- **Build Info**: Git commit, branch, and version information  
- **Summary**: Key findings and status overview
- **Details**: Comprehensive data and analysis
- **Actions**: Recommended next steps (if any)

## 📋 Quick Actions

<div class="action-grid">

### 🔍 Find Specific Information
- [Search all reports](./search.html)
- [Filter by date range](./filter.html)
- [Compare builds](./compare.html)

### 📥 Download Data
- [Export latest reports](./export.html)
- [API access documentation](./api.html)
- [Raw data files](./raw.html)

### 📊 Analytics
- [Trend analysis](./trends.html)
- [Performance dashboards](./dashboards.html)
- [Custom queries](./queries.html)

</div>

## 🎯 Report Highlights

### Security Posture
- **Current CVE Status**: ✅ No critical vulnerabilities
- **Last Security Scan**: {{ latest_date }}
- **Patch Level**: Up to date

### Build Health  
- **Success Rate**: 95% (last 30 builds)
- **Average Build Time**: 3.2 hours
- **Last Failed Build**: 2025-01-09 (dependency issue - resolved)

### License Compliance
- **Compliance Status**: ✅ Fully compliant
- **License Types**: GPL-2.0, LGPL-2.1, Apache-2.0, MIT
- **Source Availability**: 100% available

## 🔗 Related Resources

### External Documentation
- [Yocto Project CVE Database](https://www.yoctoproject.org/security/)
- [SPDX License List](https://spdx.org/licenses/)
- [Qualcomm Security Bulletins](https://www.qualcomm.com/company/product-security/bulletins)

### Integration Info
- [Main Project Repository]({{ site.project.main_repo }})
- [Yocto-Gen-Machines Hub]({{ site.project.hub_repo }})
- [Download Center](../downloads/)

---

*Reports automatically updated from build pipeline. Last refresh: {{ latest_date }} 13:44 UTC*

<style>
.report-grid > div {
    border: 1px solid #ddd;
    padding: 1.5rem;
    margin: 1rem 0;
    border-radius: 8px;
    background-color: #f9f9f9;
}

.report-grid h3 {
    color: #2c3e50;
    margin-top: 0;
}

.action-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
    margin: 2rem 0;
}

.action-grid > div {
    border: 1px solid #3498db;
    padding: 1rem;
    border-radius: 6px;
    background-color: #ecf0f1;
}

table {
    width: 100%;
    border-collapse: collapse;
    margin: 1rem 0;
}

table th, table td {
    border: 1px solid #ddd;
    padding: 0.75rem;
    text-align: left;
}

table th {
    background-color: #3498db;
    color: white;
}

table tr:nth-child(even) {
    background-color: #f2f2f2;
}

.status-success { color: #27ae60; font-weight: bold; }
.status-warning { color: #f39c12; font-weight: bold; }
.status-error { color: #e74c3c; font-weight: bold; }
</style>