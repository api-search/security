---
api_specs:
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Spot Market Data API
  slug: spot-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Derivatives API
  slug: derivatives
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata DeFi API
  slug: defi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata On-Chain API
  slug: on-chain
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-asyncapi.yml
  format: yaml
  label: Amberdata WebSocket Streaming API
  slug: websocket-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/asyncapi/amberdata-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amberdata.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amberdata.com
  spf: true
hosts:
- cert_expires: Sep 16 02:24:51 2026 GMT
  host: www.amberdata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 05:44:09 2026 GMT
  host: docs.amberdata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.amberdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amberdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amberdata, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amberdata
provider_slug: amberdata
slug: amberdata-domain-security
source_filename: amberdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amberdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.amberdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.amberdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amberdata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amberdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/security/amberdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto
- Blockchain
- Market Data
- Digital Assets
- Derivatives
- DeFi
- On-Chain
---
