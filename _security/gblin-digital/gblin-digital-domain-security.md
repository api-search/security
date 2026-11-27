---
api_specs:
- filename: gblin-digital-x402-api-openapi.yml
  format: yaml
  label: GBlin Protocol X402 API
  slug: gblin-digital-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gblin-digital/openapi/gblin-digital-x402-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gblin.digital
  spf: true
hosts:
- cert_expires: Dec 31 06:41:01 2026 GMT
  host: gblin.digital
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GBlin Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GBlin Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GBlin Protocol
provider_slug: gblin-digital
slug: gblin-digital-domain-security
source_filename: gblin-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gblin.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gblin.digital\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gblin-digital/security/gblin-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Cryptocurrency
- Tokens
- BaseNetwork
- Finance
---
