---
api_specs:
- filename: bitnomial-market-data-asyncapi.yml
  format: yaml
  label: Bitnomial Market Data WebSocket API
  slug: bitnomial-market-data-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitnomial/refs/heads/main/asyncapi/bitnomial-market-data-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitnomial.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: bitnomial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitnomial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitnomial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitnomial
provider_slug: bitnomial
slug: bitnomial-domain-security
source_filename: bitnomial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitnomial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitnomial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitnomial/refs/heads/main/security/bitnomial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Derivatives
- Exchange
- Trading
- Market Data
- Futures
- Options
- CFTC Regulated
---
