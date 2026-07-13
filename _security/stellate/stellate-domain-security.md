---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stellate.co
  spf: true
hosts:
- cert_expires: Aug  9 01:41:56 2026 GMT
  host: stellate.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:32:46 2026 GMT
  host: graph.stellate.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stellate
provider_slug: stellate
slug: stellate-domain-security
source_filename: stellate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stellate.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 01:41:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: graph.stellate.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:32:46 2026 GMT\n  hsts: null\ndomains:\n- domain: stellate.co\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellate/refs/heads/main/security/stellate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- CDN
- Edge Caching
- API Management
- Rate Limiting
- GraphQL Security
- Developer Tools
---
