---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: open-government-austria-action-api-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Action API
  slug: open-government-austria-action-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-action-api-api-openapi.yml
- filename: open-government-austria-applications-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Applications API
  slug: open-government-austria-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-applications-api-openapi.yml
- filename: open-government-austria-catalogues-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Catalogues API
  slug: open-government-austria-catalogues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-catalogues-api-openapi.yml
- filename: open-government-austria-ckan-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Ckan API
  slug: open-government-austria-ckan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-ckan-api-openapi.yml
- filename: open-government-austria-datasets-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Datasets API
  slug: open-government-austria-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-datasets-api-openapi.yml
- filename: open-government-austria-distributions-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Distributions API
  slug: open-government-austria-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-distributions-api-openapi.yml
- filename: open-government-austria-drafts-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Drafts API
  slug: open-government-austria-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-drafts-api-openapi.yml
- filename: open-government-austria-feeds-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Feeds API
  slug: open-government-austria-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-feeds-api-openapi.yml
- filename: open-government-austria-gazetteer-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Gazetteer API
  slug: open-government-austria-gazetteer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-gazetteer-api-openapi.yml
- filename: open-government-austria-identifiers-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Identifiers API
  slug: open-government-austria-identifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-identifiers-api-openapi.yml
- filename: open-government-austria-resources-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Resources API
  slug: open-government-austria-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-resources-api-openapi.yml
- filename: open-government-austria-search-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Search API
  slug: open-government-austria-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-search-api-openapi.yml
- filename: open-government-austria-sitemap-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Sitemap API
  slug: open-government-austria-sitemap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-sitemap-api-openapi.yml
- filename: open-government-austria-translation-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Translation API
  slug: open-government-austria-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-translation-api-openapi.yml
- filename: open-government-austria-vocabularies-api-openapi.yml
  format: yaml
  label: data.gv.at (Open Government Data Austria) Vocabularies API
  slug: open-government-austria-vocabularies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-government-austria/openapi/open-government-austria-vocabularies-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: data.gv.at (Open Government Data Austria) Authentication
name_suffix: Authentication
oauth_flows: []
overview: data.gv.at (Open Government Data Austria) secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: data.gv.at (Open Government Data Austria)
provider_slug: open-government-austria
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/open-government-austria-hub-repo-openapi.yml
  - openapi/open-government-austria-hub-search-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/open-government-austria-hub-repo-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth2
  parameter: Authorization
  sources:
  - openapi/open-government-austria-hub-search-openapi.yml
  type: apiKey
slug: open-government-austria-authentication
source_filename: open-government-austria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/open-government-austria-hub-repo-openapi.yml, openapi/open-government-austria-hub-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/open-government-austria-hub-repo-openapi.yml\n  - openapi/open-government-austria-hub-search-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/open-government-austria-hub-repo-openapi.yml\n- name: ApiKeyAuth2\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/open-government-austria-hub-search-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/open-government-austria/authentication/open-government-austria-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Government
- Public APIs
- Open Data
- Austria
- DCAT-AP
- Data Catalog
---
