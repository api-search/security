---
api_specs:
- filename: rtx-eagle-api-openapi.yml
  format: yaml
  label: RTX EAGLE API
  slug: eagle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtx/refs/heads/main/openapi/rtx-eagle-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuemail "sectigo.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rtx.com
  spf: true
hosts:
- cert_expires: Oct  1 10:20:19 2026 GMT
  host: www.rtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.rtx.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rtx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RTX, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RTX
provider_slug: rtx
slug: rtx-domain-security
source_filename: rtx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:20:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.rtx.com\n  https: false\ndomains:\n- domain: rtx.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuemail \"sectigo.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtx/refs/heads/main/security/rtx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Defense
- Aerospace
- Government
- Logistics
- Intelligence
- Military
---
