---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: castle.io
  spf: true
hosts:
- cert_expires: Aug 22 06:33:53 2026 GMT
  host: castle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 18:23:47 2026 GMT
  host: reference.castle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.castle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Castle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Castle
provider_slug: castle
slug: castle-domain-security
source_filename: castle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: castle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reference.castle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.castle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: castle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castle/refs/heads/main/security/castle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Fraud Prevention
- Bot Detection
- Device Fingerprinting
- Account Takeover
- Risk Scoring
- Identity
---
