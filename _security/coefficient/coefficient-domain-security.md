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
- cert_expires: Dec 11 08:22:42 2026 GMT
  host: coefficient.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coefficient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coefficient, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coefficient
provider_slug: coefficient
slug: coefficient-domain-security
source_filename: coefficient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coefficient.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 08:22:42 2026 GMT\n  hsts: false\ndomains:\n- domain: coefficient.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coefficient/refs/heads/main/security/coefficient-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Connectors
- AI Dashboards
- Spreadsheet Integration
- Revenue Operations
- Finance
- Marketing
---
