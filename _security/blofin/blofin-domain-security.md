---
api_specs:
- filename: blofin-account-api-openapi.yml
  format: yaml
  label: BloFin Account API
  slug: blofin-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-account-api-openapi.yml
- filename: blofin-affiliate-api-openapi.yml
  format: yaml
  label: BloFin Affiliate API
  slug: blofin-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-affiliate-api-openapi.yml
- filename: blofin-asset-api-openapi.yml
  format: yaml
  label: BloFin Asset API
  slug: blofin-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-asset-api-openapi.yml
- filename: blofin-copytrading-api-openapi.yml
  format: yaml
  label: BloFin Copytrading API
  slug: blofin-copytrading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-copytrading-api-openapi.yml
- filename: blofin-market-api-openapi.yml
  format: yaml
  label: BloFin Market API
  slug: blofin-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-market-api-openapi.yml
- filename: blofin-oauth-api-openapi.yml
  format: yaml
  label: BloFin OAuth API
  slug: blofin-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-oauth-api-openapi.yml
- filename: blofin-spot-api-openapi.yml
  format: yaml
  label: BloFin Spot API
  slug: blofin-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-spot-api-openapi.yml
- filename: blofin-trade-api-openapi.yml
  format: yaml
  label: BloFin Trade API
  slug: blofin-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-trade-api-openapi.yml
- filename: blofin-user-api-openapi.yml
  format: yaml
  label: BloFin User API
  slug: blofin-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blofin.com
  spf: true
hosts:
- cert_expires: Jan 10 07:34:13 2027 GMT
  host: blofin.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blofin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BloFin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BloFin
provider_slug: blofin
slug: blofin-domain-security
source_filename: blofin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blofin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 07:34:13 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blofin.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/security/blofin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Cryptocurrency Exchange
- Trading
- Futures
- Spot Trading
- Copy Trading
- WebSocket
---
