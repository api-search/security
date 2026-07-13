---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: resurface.io
  spf: true
hosts:
- cert_expires: Sep 22 00:48:07 2026 GMT
  host: resurface.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resurface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resurface, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Resurface
provider_slug: resurface
slug: resurface-domain-security
source_filename: resurface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resurface.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: resurface.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resurface/refs/heads/main/security/resurface-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Analytics
- API Compliance
- API Logging
- API Observability
- API Security
- Data Leak Prevention
- Runtime Security
- SIEM
- Threat Detection
---
