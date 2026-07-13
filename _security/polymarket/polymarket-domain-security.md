---
api_specs:
- filename: polymarket-asyncapi.yml
  format: yaml
  label: Polymarket WebSocket
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymarket/refs/heads/main/asyncapi/polymarket-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polymarket.com
  spf: true
hosts:
- cert_expires: Sep 30 10:50:18 2026 GMT
  host: polymarket.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:52:14 2026 GMT
  host: docs.polymarket.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:50:18 2026 GMT
  host: clob.polymarket.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polymarket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polymarket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polymarket
provider_slug: polymarket
slug: polymarket-domain-security
source_filename: polymarket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polymarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:50:18 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.polymarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:52:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: clob.polymarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:50:18 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: polymarket.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymarket/refs/heads/main/security/polymarket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Prediction Markets
- DeFi
- Polygon
- Order Book
- Crypto
- Markets
---
