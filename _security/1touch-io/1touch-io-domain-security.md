---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1touch.io
  spf: true
hosts:
- cert_expires: Sep 27 11:47:35 2026 GMT
  host: www.1touch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Touch Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1touch.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1touch.io
provider_slug: 1touch-io
slug: 1touch-io-domain-security
source_filename: 1touch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1touch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1touch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1touch-io/refs/heads/main/security/1touch-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Security
- Data Discovery
- Data Classification
- DSPM
- Data Governance
- Privacy
- Compliance
- Mainframe
- Access Control
- AI Security
---
