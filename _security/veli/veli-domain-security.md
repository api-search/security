---
api_specs:
- filename: veli-orders-api-openapi.yml
  format: yaml
  label: Veli Orders API
  slug: veli-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-orders-api-openapi.yml
- filename: veli-performance-api-openapi.yml
  format: yaml
  label: Veli Performance API
  slug: veli-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-performance-api-openapi.yml
- filename: veli-portfolios-api-openapi.yml
  format: yaml
  label: Veli Portfolios API
  slug: veli-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-portfolios-api-openapi.yml
- filename: veli-positions-api-openapi.yml
  format: yaml
  label: Veli Positions API
  slug: veli-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-positions-api-openapi.yml
- filename: veli-strategies-api-openapi.yml
  format: yaml
  label: Veli Strategies API
  slug: veli-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-strategies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veli.io
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: veli.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: api.veli.io
  https: false
kind: domain-security
layout: security
method: probed
name: Veli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veli, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Veli
provider_slug: veli
slug: veli-domain-security
source_filename: veli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veli.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.veli.io\n  https: false\ndomains:\n- domain: veli.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/security/veli-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Crypto
- DeFi
- Finance
- Investment
- Portfolio-Management
---
