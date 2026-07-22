---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coefficient.io
  spf: true
hosts:
- cert_expires: Oct 12 22:12:09 2026 GMT
  host: coefficient.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coefficient Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coefficient Works, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coefficient Works
provider_slug: coefficient-works
slug: coefficient-works-domain-security
source_filename: coefficient-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coefficient.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:12:09 2026 GMT\n  hsts: false\ndomains:\n- domain: coefficient.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coefficient-works/refs/heads/main/security/coefficient-works-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spreadsheets
- Google Sheets
- Microsoft Excel
- Data Integration
- No-Code
- Business Intelligence
- Reporting
- Revenue Operations
- SaaS
---
