---
api_specs:
- filename: korbit-openapi.yml
  format: yaml
  label: Korbit Open API v2
  slug: korbit-open-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-openapi.yml
- filename: korbit-websocket-asyncapi.yml
  format: yaml
  label: Korbit Open API v2 WebSocket
  slug: korbit-open-api-v2-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/asyncapi/korbit-websocket-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: korbit.co.kr
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.korbit.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: docs.korbit.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.korbit.co.kr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Korbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Korbit
provider_slug: korbit
slug: korbit-domain-security
source_filename: korbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.korbit.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: docs.korbit.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.korbit.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: korbit.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/security/korbit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Digital Assets
- Trading
- Market Data
- Financial Services
- WebSocket
- South Korea
- Blockchain
---
