---
api_specs:
- filename: qwiet-ai-openapi-original.yml
  format: yaml
  label: Qwiet AI API v4
  slug: qwiet-ai-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwiet-ai/refs/heads/main/openapi/qwiet-ai-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qwiet.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shiftleft.io
  spf: true
hosts:
- cert_expires: Sep 11 18:24:22 2026 GMT
  host: qwiet.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:41:57 2026 GMT
  host: app.shiftleft.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwiet Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwiet Ai, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qwiet Ai
provider_slug: qwiet-ai
slug: qwiet-ai-domain-security
source_filename: qwiet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qwiet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.shiftleft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:41:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qwiet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shiftleft.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwiet-ai/refs/heads/main/security/qwiet-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Application Security
- SAST
- SCA
- Code Security
- Vulnerability Management
- DevSecOps
- AutoFix
---
