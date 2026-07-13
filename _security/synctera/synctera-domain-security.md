---
api_specs:
- filename: synctera-openapi.json
  format: json
  label: Synctera Platform API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synctera/refs/heads/main/openapi/synctera-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synctera.com
  spf: true
hosts:
- cert_expires: Oct  6 19:33:34 2026 GMT
  host: synctera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:03:50 2026 GMT
  host: docs.synctera.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:31:26 2026 GMT
  host: api.synctera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synctera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synctera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synctera
provider_slug: synctera
slug: synctera-domain-security
source_filename: synctera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synctera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.synctera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.synctera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:31:26 2026 GMT\n  hsts: null\ndomains:\n- domain: synctera.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synctera/refs/heads/main/security/synctera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- KYC
---
