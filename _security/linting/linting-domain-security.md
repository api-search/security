---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: quobix.com
  spf: false
hosts:
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: stoplight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: quobix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 16:47:51 2026 GMT
  host: redocly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Linting, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: API Linting
provider_slug: linting
slug: linting-domain-security
source_filename: linting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: false\n- host: quobix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: redocly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: quobix.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linting/refs/heads/main/security/linting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Governance
- API Linting
- API Style Guide
- AsyncAPI
- JSON Schema
- Linting
- OpenAPI
- Quality Assurance
- Topic
---
