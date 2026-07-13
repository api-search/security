---
api_specs:
- filename: w3c-openapi.yml
  format: yaml
  label: W3C API
  slug: w3c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/w3c/refs/heads/main/openapi/w3c-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w3.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: whatwg.org
  spf: true
hosts:
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: www.w3.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: api.w3.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:20:30 2026 GMT
  host: html.spec.whatwg.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: W3C Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for W3C, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: W3C
provider_slug: w3c
slug: w3c-domain-security
source_filename: w3c-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: null\n- host: html.spec.whatwg.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 02:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: w3.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: whatwg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/w3c/refs/heads/main/security/w3c-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accessibility
- Standards
- Web
- Web Standards
---
