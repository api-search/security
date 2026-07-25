---
api_specs:
- filename: matrixport-account-api-openapi.yml
  format: yaml
  label: Matrixport Account API
  slug: matrixport-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-account-api-openapi.yml
- filename: matrixport-batch-orders-api-openapi.yml
  format: yaml
  label: Matrixport Batch Orders API
  slug: matrixport-batch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-batch-orders-api-openapi.yml
- filename: matrixport-block-trade-api-openapi.yml
  format: yaml
  label: Matrixport Block Trade API
  slug: matrixport-block-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-block-trade-api-openapi.yml
- filename: matrixport-market-api-openapi.yml
  format: yaml
  label: Matrixport Market API
  slug: matrixport-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-market-api-openapi.yml
- filename: matrixport-order-api-openapi.yml
  format: yaml
  label: Matrixport Order API
  slug: matrixport-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-order-api-openapi.yml
- filename: matrixport-system-api-openapi.yml
  format: yaml
  label: Matrixport System API
  slug: matrixport-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-system-api-openapi.yml
- filename: matrixport-websocket-api-openapi.yml
  format: yaml
  label: Matrixport WebSocket API
  slug: matrixport-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-websocket-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bit.com
  spf: true
hosts:
- cert_expires: Sep 20 05:25:06 2026 GMT
  host: www.bit.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.bit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Matrixport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matrixport, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matrixport
provider_slug: matrixport
slug: matrixport-domain-security
source_filename: matrixport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.bit.com\n  https: false\ndomains:\n- domain: bit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/security/matrixport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Finance
- Cryptocurrency Exchange
- Trading
- Derivatives
- Options
- Futures
- Perpetuals
- WebSocket
- REST API
---
