---
api_specs:
- filename: api-market-api-market-api-api-openapi.yml
  format: yaml
  label: API.market API.market API
  slug: api-market-api-market-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-api-market-api-api-openapi.yml
- filename: api-market-bridgeml-api-openapi.yml
  format: yaml
  label: API.market Bridgeml API
  slug: api-market-bridgeml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-bridgeml-api-openapi.yml
- filename: api-market-images-api-openapi.yml
  format: yaml
  label: API.market Images API
  slug: api-market-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-images-api-openapi.yml
- filename: api-market-magicapi-api-openapi.yml
  format: yaml
  label: API.market Magicapi API
  slug: api-market-magicapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-magicapi-api-openapi.yml
- filename: api-market-mcp-api-openapi.yml
  format: yaml
  label: API.market MCP API
  slug: api-market-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-mcp-api-openapi.yml
- filename: api-market-models-api-openapi.yml
  format: yaml
  label: API.market Models API
  slug: api-market-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-models-api-openapi.yml
- filename: api-market-pipfeed-api-openapi.yml
  format: yaml
  label: API.market Pipfeed API
  slug: api-market-pipfeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-pipfeed-api-openapi.yml
- filename: api-market-predictions-api-openapi.yml
  format: yaml
  label: API.market Predictions API
  slug: api-market-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-predictions-api-openapi.yml
- filename: api-market-status-api-openapi.yml
  format: yaml
  label: API.market Status API
  slug: api-market-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-status-api-openapi.yml
- filename: api-market-subscription-api-openapi.yml
  format: yaml
  label: API.market Subscription API
  slug: api-market-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-subscription-api-openapi.yml
- filename: api-market-toonme-api-api-openapi.yml
  format: yaml
  label: API.market Toonme API
  slug: api-market-toonme-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-toonme-api-api-openapi.yml
- filename: api-market-user-api-openapi.yml
  format: yaml
  label: API.market User API
  slug: api-market-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/openapi/api-market-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: api.market
  spf: true
hosts:
- cert_expires: Oct 29 00:46:09 2026 GMT
  host: api.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 07:44:59 2026 GMT
  host: docs.api.market
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 00:46:09 2026 GMT
  host: prod.api.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Api Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API.market, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API.market
provider_slug: api-market
slug: api-market-domain-security
source_filename: api-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 00:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.api.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 07:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.api.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 00:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: api.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/security/api-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Artificial Intelligence
- Integration
- MCP
---
