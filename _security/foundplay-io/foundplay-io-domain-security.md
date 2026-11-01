---
api_specs:
- filename: foundplay-io-games-api-openapi.yml
  format: yaml
  label: foundplay-io Games API
  slug: foundplay-io-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundplay-io/openapi/foundplay-io-games-api-openapi.yml
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
  domain: foundplay.io
  spf: true
hosts:
- cert_expires: Jan  7 20:47:47 2027 GMT
  host: foundplay.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foundplay Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for foundplay-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: foundplay-io
provider_slug: foundplay-io
slug: foundplay-io-domain-security
source_filename: foundplay-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foundplay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 20:47:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foundplay.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/foundplay-io/security/foundplay-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games
- Browser
- Indie
- AI-generated
- Free
---
