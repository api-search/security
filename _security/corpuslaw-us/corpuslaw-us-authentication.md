---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corpuslaw-us-account-api-openapi.yml
  format: yaml
  label: Corpus Account API
  slug: corpuslaw-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-account-api-openapi.yml
- filename: corpuslaw-us-browse-api-openapi.yml
  format: yaml
  label: Corpus Browse API
  slug: corpuslaw-us-browse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-browse-api-openapi.yml
- filename: corpuslaw-us-coverage-api-openapi.yml
  format: yaml
  label: Corpus Coverage API
  slug: corpuslaw-us-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-coverage-api-openapi.yml
- filename: corpuslaw-us-formation-api-openapi.yml
  format: yaml
  label: Corpus Formation API
  slug: corpuslaw-us-formation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-formation-api-openapi.yml
- filename: corpuslaw-us-general-api-openapi.yml
  format: yaml
  label: Corpus General API
  slug: corpuslaw-us-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-general-api-openapi.yml
- filename: corpuslaw-us-gis-api-openapi.yml
  format: yaml
  label: Corpus GIS API
  slug: corpuslaw-us-gis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-gis-api-openapi.yml
- filename: corpuslaw-us-search-api-openapi.yml
  format: yaml
  label: Corpus Search API
  slug: corpuslaw-us-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Corpus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corpus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Corpus
provider_slug: corpuslaw-us
scheme_count: 1
schemes:
- description: 'Pass your key as `Authorization: Bearer <api_key>`. Header only — query-param auth is disabled in production.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/corpuslaw-us-openapi.yml
  type: http
slug: corpuslaw-us-authentication
source_filename: corpuslaw-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corpuslaw.us/docs/api.md\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your key as `Authorization: Bearer <api_key>`. Header only —\n    query-param auth is disabled in production.'\n  sources:\n  - openapi/corpuslaw-us-openapi.yml\ndocs: https://corpuslaw.us/docs/api\nnotes:\n- Keys (cp_…) are self-serve and instant at https://corpuslaw.us/settings, no review\n  step and no expiry.\n- Query-parameter auth (?api_key=) is disabled in production.\n- MCP server at https://corpuslaw.us/api/mcp needs no auth; adding the Bearer header\n  raises the allotment.\n- Widget uses a separate publishable widget key (pk_…).\n"
source_yaml_url: https://artifacts.apis.io/corpuslaw-us/authentication/corpuslaw-us-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Legal
- Law
- Business Formation
- LLC
- Compliance
- MCP
- AI Agents
---
