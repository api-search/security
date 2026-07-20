---
api_key_in:
- header
api_specs:
- filename: chaitin-safeline-openapi-original.json
  format: json
  label: SafeLine WAF Open API
  slug: safeline-waf-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-safeline-openapi-original.json
- filename: chaitin-cloudatlas-openapi-original.yaml
  format: yaml
  label: Cloud Atlas OpenAPI
  slug: cloud-atlas-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-cloudatlas-openapi-original.yaml
- filename: chaitin-apisec-openapi-original.json
  format: json
  label: APISec Management API
  slug: apisec-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-apisec-openapi-original.json
- filename: chaitin-veinmind-openapi-original.json
  format: json
  label: VeinMind API
  slug: veinmind-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-veinmind-openapi-original.json
- filename: chaitin-ddr-openapi-original.json
  format: json
  label: DDR API
  slug: ddr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-ddr-openapi-original.json
- filename: chaitin-dsensor-openapi-original.json
  format: json
  label: D-Sensor API
  slug: d-sensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-dsensor-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chaitin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chaitin Tech secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chaitin Tech
provider_slug: chaitin
scheme_count: 2
schemes:
- docs: https://docs.waf.chaitin.com/en/tech_docs/OPENAPI
  in: header
  min_version: 6.6.0
  name: X-SLCE-API-TOKEN
  parameter: X-SLCE-API-TOKEN
  product: SafeLine WAF
  sources:
  - openapi/chaitin-safeline-openapi-original.json
  token_endpoint: SafeLine console -> System Management -> API Token
  type: apiKey
- in: header
  name: apikey-header-TOKEN
  parameter: TOKEN
  product: Cloud Atlas
  sources:
  - openapi/chaitin-cloudatlas-openapi-original.yaml
  type: apiKey
slug: chaitin-authentication
source_filename: chaitin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/chaitin-cloudatlas-openapi-original.yaml\ndocs: https://docs.waf.chaitin.com/en/tech_docs/OPENAPI\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Chaitin products are self-hosted / cloud appliances that authenticate API\n    clients with a per-instance API token passed in a request header. SafeLine\n    WAF uses the X-SLCE-API-TOKEN header against the Open API on port 9443\n    (/api/open/*); Cloud Atlas uses a TOKEN header. Tokens are minted in each\n    product's System / API Token console. No OAuth2 / OIDC surface is exposed on\n    the machine APIs (OIDC in SafeLine is console SSO, not API auth).\nschemes:\n- name: X-SLCE-API-TOKEN\n  type: apiKey\n  in: header\n  parameter: X-SLCE-API-TOKEN\n  product: SafeLine WAF\n  min_version: '6.6.0'\n  token_endpoint: SafeLine console -> System Management -> API Token\n  docs: https://docs.waf.chaitin.com/en/tech_docs/OPENAPI\n  sources:\n  -\
  \ openapi/chaitin-safeline-openapi-original.json\n- name: apikey-header-TOKEN\n  type: apiKey\n  in: header\n  parameter: TOKEN\n  product: Cloud Atlas\n  sources:\n  - openapi/chaitin-cloudatlas-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/authentication/chaitin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Security
- Web Application Firewall
- WAF
- Cybersecurity
- API Security
- Container Security
- Vulnerability Scanning
- DevSecOps
- Company
---
