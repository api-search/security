---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: syspro.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.syspro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: help.syspro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: developer.syspro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syspro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SYSPRO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SYSPRO
provider_slug: syspro
slug: syspro-domain-security
source_filename: syspro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syspro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.syspro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: developer.syspro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: syspro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syspro/refs/heads/main/security/syspro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Manufacturing
- Distribution
- Inventory
- Production Orders
- Purchasing
- Sales
- Financial Accounting
- Supply Chain
---
