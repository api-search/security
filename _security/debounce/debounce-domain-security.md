---
api_specs:
- filename: debounce-email-validation-api-openapi.yml
  format: yaml
  label: DeBounce Email Validation API
  slug: email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-email-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: debounce.com
  spf: true
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
  domain: debounce.io
  spf: true
hosts:
- cert_expires: Aug 17 22:26:01 2026 GMT
  host: debounce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 09:17:08 2026 GMT
  host: api.debounce.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeBounce, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeBounce
provider_slug: debounce
slug: debounce-domain-security
source_filename: debounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: debounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:26:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.debounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:17:08 2026 GMT\n  hsts: null\ndomains:\n- domain: debounce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: debounce.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/security/debounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
---
