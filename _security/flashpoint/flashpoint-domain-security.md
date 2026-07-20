---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flashpoint.io
  spf: true
hosts:
- cert_expires: Sep 29 04:13:22 2026 GMT
  host: flashpoint.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:01:00 2026 GMT
  host: docs.flashpoint.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:13:22 2026 GMT
  host: api.flashpoint.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flashpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flashpoint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flashpoint
provider_slug: flashpoint
slug: flashpoint-domain-security
source_filename: flashpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flashpoint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:13:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flashpoint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flashpoint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:13:22 2026 GMT\n  hsts: null\ndomains:\n- domain: flashpoint.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flashpoint/refs/heads/main/security/flashpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Threat Intelligence
- Cybersecurity
- Security
- Fraud Prevention
- Vulnerability Management
- Dark Web
- Data
---
