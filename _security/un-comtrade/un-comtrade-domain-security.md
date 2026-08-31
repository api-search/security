---
api_specs:
- filename: un-comtrade-bulk-download-api-openapi.yml
  format: yaml
  label: UN Comtrade Bulk Download API
  slug: un-comtrade-bulk-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-bulk-download-api-openapi.yml
- filename: un-comtrade-data-availability-api-openapi.yml
  format: yaml
  label: UN Comtrade Data Availability API
  slug: un-comtrade-data-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-data-availability-api-openapi.yml
- filename: un-comtrade-final-trade-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Final Trade Data API
  slug: un-comtrade-final-trade-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-final-trade-data-api-openapi.yml
- filename: un-comtrade-public-preview-api-openapi.yml
  format: yaml
  label: UN Comtrade Public Preview API
  slug: un-comtrade-public-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-public-preview-api-openapi.yml
- filename: un-comtrade-reference-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Reference Data API
  slug: un-comtrade-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-reference-data-api-openapi.yml
- filename: un-comtrade-tariffline-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Tariffline Data API
  slug: un-comtrade-tariffline-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-tariffline-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: un.org
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: comtradeapi.un.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Un Comtrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UN Comtrade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UN Comtrade
provider_slug: un-comtrade
slug: un-comtrade-domain-security
source_filename: un-comtrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comtradeapi.un.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: un.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/security/un-comtrade-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Trade
- International Trade
- Import
- Export
- Statistics
- United Nations
- Economics
- Commodities
- Bilateral Trade
- HS Codes
- SITC
---
