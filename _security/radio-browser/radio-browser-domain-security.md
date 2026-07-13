---
api_specs:
- filename: radio-browser-openapi.yml
  format: yaml
  label: Radio Browser API
  slug: radio-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radio-browser/refs/heads/main/openapi/radio-browser-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: radio-browser.info
  spf: false
hosts:
- cert_expires: Oct  2 04:33:48 2026 GMT
  host: www.radio-browser.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:03:43 2026 GMT
  host: api.radio-browser.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 19:24:46 2026 GMT
  host: de1.api.radio-browser.info
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Radio Browser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radio Browser, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Radio Browser
provider_slug: radio-browser
slug: radio-browser-domain-security
source_filename: radio-browser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.radio-browser.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.radio-browser.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: de1.api.radio-browser.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:24:46 2026 GMT\n  hsts: null\ndomains:\n- domain: radio-browser.info\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radio-browser/refs/heads/main/security/radio-browser-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Music
- Radio
- Streaming
- Open Source
- Open Data
- Community
- Public APIs
- AGPL
---
