---
api_specs:
- filename: bitvavo-exchange-websocket-asyncapi.yml
  format: yaml
  label: Bitvavo WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/asyncapi/bitvavo-exchange-websocket-asyncapi.yml
- filename: bitvavo-market-data-pro-asyncapi.yml
  format: yaml
  label: Bitvavo Market Data Pro WebSocket API
  slug: market-data-pro-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/asyncapi/bitvavo-market-data-pro-asyncapi.yml
- filename: bitvavo-account-api-openapi.yml
  format: yaml
  label: Bitvavo Account API
  slug: bitvavo-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-account-api-openapi.yml
- filename: bitvavo-account-management-api-openapi.yml
  format: yaml
  label: Bitvavo Account Management API
  slug: bitvavo-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-account-management-api-openapi.yml
- filename: bitvavo-market-data-api-openapi.yml
  format: yaml
  label: Bitvavo Market data API
  slug: bitvavo-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-market-data-api-openapi.yml
- filename: bitvavo-subaccounts-api-openapi.yml
  format: yaml
  label: Bitvavo Subaccounts API
  slug: bitvavo-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-subaccounts-api-openapi.yml
- filename: bitvavo-synchronization-api-openapi.yml
  format: yaml
  label: Bitvavo Synchronization API
  slug: bitvavo-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-synchronization-api-openapi.yml
- filename: bitvavo-trading-api-openapi.yml
  format: yaml
  label: Bitvavo Trading API
  slug: bitvavo-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-trading-api-openapi.yml
- filename: bitvavo-transfer-api-openapi.yml
  format: yaml
  label: Bitvavo Transfer API
  slug: bitvavo-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-transfer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitvavo.com
  spf: true
hosts:
- cert_expires: Dec 10 03:59:01 2026 GMT
  host: bitvavo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitvavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitvavo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitvavo
provider_slug: bitvavo
slug: bitvavo-domain-security
source_filename: bitvavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitvavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:59:01 2026 GMT\n  hsts: null\ndomains:\n- domain: bitvavo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/security/bitvavo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Netherlands
---
