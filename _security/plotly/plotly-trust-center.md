---
certifications:
- SOC 2 Type I
- SOC 2 Type II
- ISO/IEC 27001
- ISO/IEC 27701
- ISO/IEC 42001
description: ''
kind: trust-center
layout: security
name: Plotly Trust Center
name_suffix: Trust Center
overview: Plotly maintains a public trust center documenting SOC 2 Type I, SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27701, and ISO/IEC 42001 compliance.
provider_name: Plotly
provider_slug: plotly
slug: plotly-trust-center
source_filename: plotly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://trust.plotly.com/ and https://plotly.com/security/\ntrust_center:\n  url: https://trust.plotly.com/\n  status: 200\n  platform: Anecdotes\n  platform_evidence: 'og:title meta tag reads \"Trust Center | Powered by Anecdotes\"'\n  machine_readable: false\n  note: >-\n    trust.plotly.com returns HTTP 200 but the body is an Angular single-page-app shell\n    (apps/trustcenter/main.*.js); no certification content is present in the served HTML, so an\n    agent or crawler reading the page gets a title and nothing else. The certifications recorded\n    below are therefore sourced from https://plotly.com/security/ and https://plotly.com/pricing/,\n    which state them in server-rendered text.\ncertifications:\n- name: SOC 2 Type I\n  source: https://plotly.com/security/\n  statement: Our organization is also SOC 2 Type I and II compliant.\n- name: SOC 2 Type II\n  source: https://plotly.com/security/\n- name: ISO/IEC 27001\n\
  \  source: https://plotly.com/security/\n  also_listed: https://plotly.com/pricing/ (Enterprise tier)\n- name: ISO/IEC 27701\n  source: https://plotly.com/security/\n  also_listed: https://plotly.com/pricing/ (Enterprise tier)\n  scope: Privacy information management\n- name: ISO/IEC 42001\n  source: https://plotly.com/security/\n  also_listed: https://plotly.com/pricing/ (Enterprise tier)\n  scope: AI management system\ninfrastructure_accreditations:\n  provider: AWS\n  note: >-\n    Inherited from the hosting provider and listed as such on Plotly's security page, not earned\n    by Plotly - recorded separately so they are not double-counted as Plotly certifications.\n  items:\n  - SOC 1 / SOC 2 / SSAE 16 / ISAE 3402\n  - ISO 27001\n  - PCI DSS Level 1\n  - FISMA Moderate\n  - Sarbanes-Oxley (SOX)\ndata_practices:\n  hosting: AWS\n  telemetry: Limited telemetry collected for service improvement\n  retention: Based on legal obligations and business interests\nsecurity_contact: security@plotly.com\n\
  x-evidence:\n- url: https://trust.plotly.com/\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://plotly.com/security/\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://plotly.com/pricing/\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotly/refs/heads/main/security/plotly-trust-center.yml
summary_line: SOC 2 Type I, SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27701, ISO/IEC 42001
tags:
- Company
- Data Visualization
- Analytics
- Data Apps
- Business Intelligence
- Open Source
- Python
- JavaScript
- Charts
- Dashboards
- Developer Tools
- MCP
trust_url: ''
---
