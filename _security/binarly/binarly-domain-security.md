---
api_specs:
- filename: binarly-openapi-original.yml
  format: yaml
  label: Binarly Transparency Platform API
  slug: binarly-transparency-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: binarly.io
  spf: true
hosts:
- cert_expires: Aug 21 12:25:29 2026 GMT
  host: docs.binarly.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binarly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binarly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Binarly
provider_slug: binarly
slug: binarly-domain-security
source_filename: binarly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.binarly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:25:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: binarly.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/security/binarly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Firmware Security
- Supply Chain Security
- Vulnerability Management
- SBOM
- Binary Analysis
- Post-Quantum Cryptography
- UEFI
- DevSecOps
---
