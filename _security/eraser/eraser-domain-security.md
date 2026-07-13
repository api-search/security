---
api_specs:
- filename: api-spec.json
  format: json
  label: Eraser API
  slug: eraser-api
  spec_type: OpenAPI
  url: https://app.eraser.io/.well-known/api-spec.json
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
  dmarc_policy: none
  dnssec: false
  domain: eraser.io
  spf: true
hosts:
- cert_expires: Aug 13 17:00:20 2026 GMT
  host: www.eraser.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:44:58 2026 GMT
  host: docs.eraser.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 00:58:26 2026 GMT
  host: app.eraser.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eraser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eraser, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eraser
provider_slug: eraser
slug: eraser-domain-security
source_filename: eraser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eraser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:00:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.eraser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:44:58 2026 GMT\n  hsts: null\n- host: app.eraser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:58:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eraser.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/security/eraser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Diagrams
- Documentation
- AI
- Technical Documentation
- Diagramming
- Architecture
- Developer Tools
---
