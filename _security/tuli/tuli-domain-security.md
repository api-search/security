---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tuli.health
  spf: true
hosts:
- cert_expires: Aug  8 00:14:48 2026 GMT
  host: tuli.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tuli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tuli
provider_slug: tuli
slug: tuli-domain-security
source_filename: tuli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tuli.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 00:14:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tuli.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuli/refs/heads/main/security/tuli-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Diagnostics
- Blood Testing
- Phlebotomy
- Pharmacy
- Health Tech
- United Kingdom
---
