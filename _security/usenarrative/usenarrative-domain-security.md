---
api_specs:
- filename: usenarrative-sports-openapi-original.json
  format: json
  label: Narrative Sports API
  slug: narrative-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usenarrative/refs/heads/main/openapi/usenarrative-sports-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: narrative-sports.com
  spf: true
hosts:
- cert_expires: Sep  8 00:57:03 2026 GMT
  host: www.narrative-sports.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 00:57:03 2026 GMT
  host: api.narrative-sports.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usenarrative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Narrative Sports, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Narrative Sports
provider_slug: usenarrative
slug: usenarrative-domain-security
source_filename: usenarrative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.narrative-sports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 00:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.narrative-sports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 00:57:03 2026 GMT\n  hsts: null\ndomains:\n- domain: narrative-sports.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usenarrative/refs/heads/main/security/usenarrative-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Video
- Artificial Intelligence
- Highlights
- Broadcasting
- Media
- Sports Technology
---
