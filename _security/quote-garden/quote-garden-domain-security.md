---
api_specs:
- filename: quote-garden-openapi.yml
  format: yaml
  label: Quote Garden REST API
  slug: quote-garden-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quote-garden/refs/heads/main/openapi/quote-garden-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onrender.com
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: herokuapp.com
  spf: false
hosts:
- cert_expires: Aug 24 22:01:50 2026 GMT
  host: quote-garden.onrender.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: quote-garden.herokuapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quote Garden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quote Garden, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Quote Garden
provider_slug: quote-garden
slug: quote-garden-domain-security
source_filename: quote-garden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quote-garden.onrender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:01:50 2026 GMT\n  hsts: null\n- host: quote-garden.herokuapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: onrender.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: herokuapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quote-garden/refs/heads/main/security/quote-garden-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Quotes
- Inspiration
- Open Source
- Free API
- Node.js
- MongoDB
- Express
- Personality
- Public APIs
---
