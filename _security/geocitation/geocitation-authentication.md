---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: geocitation-audits-api-openapi.yml
  format: yaml
  label: GEOCitation Audits API
  slug: geocitation-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-audits-api-openapi.yml
- filename: geocitation-gdpr-api-openapi.yml
  format: yaml
  label: GEOCitation Gdpr API
  slug: geocitation-gdpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-gdpr-api-openapi.yml
- filename: geocitation-health-api-openapi.yml
  format: yaml
  label: GEOCitation Health API
  slug: geocitation-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-health-api-openapi.yml
- filename: geocitation-meta-api-openapi.yml
  format: yaml
  label: GEOCitation Meta API
  slug: geocitation-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-meta-api-openapi.yml
- filename: geocitation-opt-out-api-openapi.yml
  format: yaml
  label: GEOCitation Opt Out API
  slug: geocitation-opt-out-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-opt-out-api-openapi.yml
- filename: geocitation-usage-api-openapi.yml
  format: yaml
  label: GEOCitation Usage API
  slug: geocitation-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-usage-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Geocitation Authentication
name_suffix: Authentication
oauth_flows: []
overview: GEOCitation secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GEOCitation
provider_slug: geocitation
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/geocitation-openapi.json
  type: http
- evidence: 'live 401 WWW-Authenticate: Bearer, ApiKey; docs example -H "X-API-Key: geo_citation_YOUR_KEY"'
  in: header
  key_prefix: geo_citation_
  name: ApiKeyHeader
  parameter_name: X-API-Key
  source: https://www.geocitation.io/en/documentation
  type: apiKey
slug: geocitation-authentication
source_filename: geocitation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/geocitation-openapi.json\ndocs: https://www.geocitation.io/en/documentation\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The OpenAPI declares only HTTPBearer (http/bearer), but the live API and the\n    published docs accept an API key in the X-API-Key header (keys are prefixed\n    \"geo_citation_\"). An unauthenticated request to https://api.geocitation.io/v1/usage\n    returns 401 with `WWW-Authenticate: Bearer, ApiKey`, confirming both schemes.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/geocitation-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  key_prefix: geo_citation_\n  source: https://www.geocitation.io/en/documentation\n  evidence: 'live 401 WWW-Authenticate: Bearer, ApiKey; docs example -H \"X-API-Key: geo_citation_YOUR_KEY\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/authentication/geocitation-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- SEO
- Geo
- AEO
- AI Search Visibility
- Content Intelligence
- Competitive Intelligence
- Marketing
- MarTech
- White Label
- Agency Tooling
- Web Data & Analytics
---
