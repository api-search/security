---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cactos.com
  spf: true
hosts:
- cert_expires: Nov  9 13:00:14 2026 GMT
  host: cactos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cactosaa16 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cactosaa16, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cactosaa16
provider_slug: cactosaa16
slug: cactosaa16-domain-security
source_filename: cactosaa16-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cactos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 13:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cactos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cactosaa16/refs/heads/main/security/cactosaa16-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Storage
- Finland
- Startup
- Battery
- Company
---
