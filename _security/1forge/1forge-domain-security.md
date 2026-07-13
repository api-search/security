---
api_specs:
- filename: 1forge-forex-data-api.yml
  format: yaml
  label: 1Forge Forex Data API
  slug: 1forge-forex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/openapi/1forge-forex-data-api.yml
- filename: 1forge-forex-stream-asyncapi.yml
  format: yaml
  label: 1Forge Forex Stream
  slug: 1forge-forex-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/asyncapi/1forge-forex-stream-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1forge.com
  spf: true
hosts:
- cert_expires: Sep 25 23:45:27 2026 GMT
  host: 1forge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.1forge.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: sockets.1forge.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 1Forge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Forge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1Forge
provider_slug: 1forge
slug: 1forge-domain-security
source_filename: 1forge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1forge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:45:27 2026 GMT\n  hsts: false\n- host: api.1forge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\n- host: sockets.1forge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 1forge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/security/1forge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency Exchange
- Forex
- Cryptocurrency
- Market Data
- Financial Data
- Real-Time Data
---
