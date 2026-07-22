---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: observablehq.com
  spf: true
hosts:
- cert_expires: Sep 25 19:15:09 2026 GMT
  host: observablehq.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Observable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Observable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Observable
provider_slug: observable
slug: observable-domain-security
source_filename: observable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: observablehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:15:09 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: observablehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observable/refs/heads/main/security/observable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Visualization
- Data Analysis
- Business Intelligence
- Notebooks
- Dashboards
- Developer Tools
- JavaScript
- D3
---
