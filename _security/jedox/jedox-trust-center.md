---
certifications: []
description: ''
kind: trust-center
layout: security
name: Jedox Trust Center
name_suffix: Trust Center
overview: Jedox maintains a public trust center covering its security and compliance posture.
provider_name: Jedox
provider_slug: jedox
slug: jedox-trust-center
source_filename: jedox-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://trust.jedox.com/\nprobe: true\nurl: https://trust.jedox.com/\nplatform: UpGuard Trust Center\nverified: true\ncertifications: []\nnote: >-\n  trust.jedox.com resolves to an UpGuard-hosted Trust Center\n  (customer.trust.upguard.com) and is linked from the jedox.com homepage footer,\n  confirming a real, published trust center. The certification/document list is\n  rendered client-side (JavaScript SPA) and could not be extracted server-side,\n  so specific named certifications are intentionally left empty rather than\n  fabricated. A future authenticated/rendered fetch can enumerate the SOC/ISO\n  documents Jedox publishes there. No `Compliance` pointer is emitted because no\n  named certification could be verified in this pass.\nevidence:\n- source: https://trust.jedox.com/\n  kind: trust-center\n  detail: UpGuard Trust Center page (HTTP 200), linked from jedox.com homepage\n- source: dns\n  kind: cname\n  detail: trust.jedox.com\
  \ -> customer.trust.upguard.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jedox/refs/heads/main/security/jedox-trust-center.yml
summary_line: trust center published
tags:
- Company
- Enterprise Performance Management
- Financial Planning and Analysis
- Budgeting and Forecasting
- Business Intelligence
- OLAP
- Integrated Business Planning
- Data Integration
- Reporting
- Analytics
trust_url: https://trust.jedox.com/
---
