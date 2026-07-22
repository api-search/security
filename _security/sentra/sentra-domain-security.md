---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sentra.io
  spf: true
hosts:
- cert_expires: Aug 29 11:27:08 2026 GMT
  host: www.sentra.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sentra
provider_slug: sentra
slug: sentra-domain-security
source_filename: sentra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:27:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sentra.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentra/refs/heads/main/security/sentra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Data Security
- DSPM
- Data Security Posture Management
- Cloud Security
- Data Classification
- AI Security
---
