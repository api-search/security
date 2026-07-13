---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logility.com
  spf: true
hosts:
- cert_expires: Sep  5 09:24:09 2026 GMT
  host: www.logility.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.logility.com
  https: false
kind: domain-security
layout: security
method: probed
name: Logility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logility, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logility
provider_slug: logility
slug: logility-domain-security
source_filename: logility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.logility.com\n  https: false\ndomains:\n- domain: logility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logility/refs/heads/main/security/logility-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Demand Planning
- Inventory Optimization
- Supply Planning
- S&OP
- Supply Chain Analytics
- AI
- Machine Learning
---
