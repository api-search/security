---
api_specs:
- filename: qwiet-api-original.yml
  format: yaml
  label: Qwiet API
  slug: qwiet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwiet/refs/heads/main/openapi/qwiet-api-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shiftleft.io
  spf: true
hosts:
- cert_expires: Sep 25 00:33:36 2026 GMT
  host: www.shiftleft.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwiet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwiet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qwiet
provider_slug: qwiet
slug: qwiet-domain-security
source_filename: qwiet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shiftleft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:33:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shiftleft.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwiet/refs/heads/main/security/qwiet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Application Security
- SAST
- SCA
- Vulnerability Management
- DevSecOps
- Code Analysis
- MCP
---
