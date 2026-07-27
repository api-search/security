---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adunaglobal.com
  spf: true
hosts:
- cert_expires: Aug 28 03:49:14 2026 GMT
  host: adunaglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aduna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aduna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aduna
provider_slug: aduna
slug: aduna-domain-security
source_filename: aduna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adunaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:49:14 2026 GMT\n  hsts: false\ndomains:\n- domain: adunaglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aduna/refs/heads/main/security/aduna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- Sweden
- Network APIs
- CAMARA
- Open Gateway
- API Aggregator
- Identity Verification
- SIM Swap
- Number Verification
- Fraud Prevention
- Quality on Demand
- Device Location
- Ericsson
---
