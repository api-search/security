---
api_specs:
- filename: finage-openapi.yml
  format: yaml
  label: Finage Market Data API
  slug: finage-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/openapi/finage-openapi.yml
- filename: finage-websocket-asyncapi.yml
  format: yaml
  label: Finage WebSocket Market Data Stream
  slug: finage-websocket-market-data-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/asyncapi/finage-websocket-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finage.co.uk
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: finage.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Finage
provider_slug: finage
slug: finage-domain-security
source_filename: finage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finage.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: finage.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/security/finage-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Market Data
- Stocks
- Forex
- Cryptocurrency
- ETFs
- Indices
- Fundamentals
- Real-Time Data
- Public APIs
---
