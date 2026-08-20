---
api_specs:
- filename: zillapi-account-api-openapi.yml
  format: yaml
  label: Zillapi Account API
  slug: zillapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-account-api-openapi.yml
- filename: zillapi-buildings-api-openapi.yml
  format: yaml
  label: Zillapi Buildings API
  slug: zillapi-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-buildings-api-openapi.yml
- filename: zillapi-jobs-api-openapi.yml
  format: yaml
  label: Zillapi Jobs API
  slug: zillapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-jobs-api-openapi.yml
- filename: zillapi-listings-api-openapi.yml
  format: yaml
  label: Zillapi Listings API
  slug: zillapi-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-listings-api-openapi.yml
- filename: zillapi-properties-api-openapi.yml
  format: yaml
  label: Zillapi Properties API
  slug: zillapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-properties-api-openapi.yml
- filename: zillapi-search-api-openapi.yml
  format: yaml
  label: Zillapi Search API
  slug: zillapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-search-api-openapi.yml
- filename: zillapi-webhooks-api-openapi.yml
  format: yaml
  label: Zillapi Webhooks API
  slug: zillapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zillapi.com
  spf: true
hosts:
- cert_expires: Sep 29 09:08:40 2026 GMT
  host: zillapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:56:33 2026 GMT
  host: api.zillapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zillapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zillapi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zillapi
provider_slug: zillapi
slug: zillapi-domain-security
source_filename: zillapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zillapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:08:40 2026 GMT\n  hsts: false\n- host: api.zillapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:56:33 2026 GMT\n  hsts: false\ndomains:\n- domain: zillapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/security/zillapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- PropTech
- Property Data
- Zillow
- Zestimate
- Valuation
- AVM
- Listings
- MCP
- AI Agent
- REST API
---
