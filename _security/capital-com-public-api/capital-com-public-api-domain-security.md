---
api_specs:
- filename: capital-com-public-api-capital-com-rest-api-openapi.yml
  format: yaml
  label: Capital.com REST API
  slug: capital-com-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/openapi/capital-com-public-api-capital-com-rest-api-openapi.yml
- filename: capital-com-public-api-asyncapi.yml
  format: yaml
  label: Capital.com WebSocket API
  slug: capital-com-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/asyncapi/capital-com-public-api-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: capital.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: backend-capital.com
  spf: false
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: capital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:14:34 2026 GMT
  host: open-api.capital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 25 11:30:14 2026 GMT
  host: api-capital.backend-capital.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capital Com Public Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capital.com Public API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Capital.com Public API
provider_slug: capital-com-public-api
slug: capital-com-public-api-domain-security
source_filename: capital-com-public-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-api.capital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:14:34 2026 GMT\n  hsts: false\n- host: api-capital.backend-capital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 11:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: capital.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: backend-capital.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/security/capital-com-public-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CFD
- Commodities
- Cryptocurrency
- Financial
- Forex
- Indices
- Market Data
- Shares
- Streaming
- Trading
- WebSocket
---
