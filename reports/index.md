---
layout: default
title: "Reports Dashboard"
description: "Comprehensive reports for QCM6490-KIT builds including security, licensing, and performance data"
---

# Reports Dashboard

Welcome to the QCM6490-KIT reports center. Here you'll find comprehensive information about builds, security, licensing, and performance metrics.

## 📊 Report Categories

<div class="report-grid">

<div>
<h3>🔨 Build Reports</h3>
<p><strong>Latest build status and detailed logs</strong></p>
<ul>
<li>Build success/failure status</li>
<li>Compilation logs and error analysis</li>
<li>Package manifests and dependency trees</li>
<li>Build artifacts and size analysis</li>
</ul>
<p><a href="./builds/">📁 View Build Reports</a> | <a href="./builds/latest.html">📄 Latest Build</a></p>
</div>

<div>
<h3>🔒 Security Reports</h3>
<p><strong>CVE analysis and vulnerability tracking</strong></p>
<ul>
<li>Known vulnerabilities assessment</li>
<li>Security patches and updates</li>
<li>Attack surface analysis</li>
<li>Compliance status reports</li>
</ul>
<p><a href="./cve/">🛡️ View Security Reports</a> | <a href="./cve/latest.html">🔍 Latest CVE Analysis</a></p>
</div>

<div>
<h3>📋 License Reports</h3>
<p><strong>Legal compliance and license information</strong></p>
<ul>
<li>Complete license inventory</li>
<li>GPL/LGPL/Apache/MIT compliance</li>
<li>Source code availability</li>
<li>Legal review summaries</li>
</ul>
<p><a href="./licenses/">⚖️ View License Reports</a> | <a href="./licenses/latest.html">📜 Latest License Report</a></p>
</div>

<div>
<h3>📈 Performance Statistics</h3>
<p><strong>Build metrics and performance trends</strong></p>
<ul>
<li>Build time trends</li>
<li>Resource usage analysis</li>
<li>Artifact size tracking</li>
<li>Success rate metrics</li>
</ul>
<p><a href="./statistics/">📊 View Statistics</a> | <a href="./statistics/latest.html">📈 Latest Stats</a></p>
</div>

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

<div>
<h3>🔍 Find Specific Information</h3>
<ul>
<li><a href="./search.html">Search all reports</a></li>
<li><a href="./filter.html">Filter by date range</a></li>
<li><a href="./compare.html">Compare builds</a></li>
</ul>
</div>

<div>
<h3>📥 Download Data</h3>
<ul>
<li><a href="./export.html">Export latest reports</a></li>
<li><a href="./api.html">API access documentation</a></li>
<li><a href="./raw.html">Raw data files</a></li>
</ul>
</div>

<div>
<h3>📊 Analytics</h3>
<ul>
<li><a href="./trends.html">Trend analysis</a></li>
<li><a href="./dashboards.html">Performance dashboards</a></li>
<li><a href="./queries.html">Custom queries</a></li>
</ul>
</div>

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