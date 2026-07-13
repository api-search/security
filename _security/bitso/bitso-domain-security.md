---
api_specs:
- filename: llms.txt
  format: yaml
  label: Bitso Trading REST API (v3)
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.bitso.com/llms.txt
- filename: bitso-asyncapi.yml
  format: yaml
  label: Bitso WebSocket API
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitso/refs/heads/main/asyncapi/bitso-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitso.com
  spf: true
hosts:
- cert_expires: Oct  7 11:34:32 2026 GMT
  host: bitso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 09:31:54 2026 GMT
  host: docs.bitso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:51:43 2026 GMT
  host: api.bitso.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitso, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitso
provider_slug: bitso
slug: bitso-domain-security
source_filename: bitso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:34:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.bitso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 09:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bitso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:51:43 2026 GMT\n  hsts: null\ndomains:\n- domain: bitso.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitso/refs/heads/main/security/bitso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Stablecoins
- Payouts
- Cross Border
- Latin America
- Mexico
- Fintech
---
