---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ctrl-tx.com
  spf: true
hosts:
- cert_expires: Oct  2 23:40:41 2026 GMT
  host: ctrl-tx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ctrl Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CTRL Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CTRL Therapeutics
provider_slug: ctrl-therapeutics
slug: ctrl-therapeutics-domain-security
source_filename: ctrl-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ctrl-tx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:40:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ctrl-tx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctrl-therapeutics/refs/heads/main/security/ctrl-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- Cancer
- Healthcare
- Life Sciences
- Pharmaceuticals
---
