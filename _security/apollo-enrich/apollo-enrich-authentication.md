---
api_key_in: []
api_specs:
- filename: apollo-enrich-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Accounts API
  slug: apollo-enrich-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-accounts-api-openapi.yml
- filename: apollo-enrich-contacts-api-openapi.yml
  format: yaml
  label: Apollo.io Contacts API
  slug: apollo-enrich-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-contacts-api-openapi.yml
- filename: apollo-enrich-organization-enrichment-api-openapi.yml
  format: yaml
  label: Apollo.io Organization Enrichment API
  slug: apollo-enrich-organization-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-organization-enrichment-api-openapi.yml
- filename: apollo-enrich-organization-search-api-openapi.yml
  format: yaml
  label: Apollo.io Organization Search API
  slug: apollo-enrich-organization-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-organization-search-api-openapi.yml
- filename: apollo-enrich-people-enrichment-api-openapi.yml
  format: yaml
  label: Apollo.io People Enrichment API
  slug: apollo-enrich-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-people-enrichment-api-openapi.yml
- filename: apollo-enrich-people-search-api-openapi.yml
  format: yaml
  label: Apollo.io People Search API
  slug: apollo-enrich-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-people-search-api-openapi.yml
- filename: apollo-enrich-sequences-api-openapi.yml
  format: yaml
  label: Apollo.io Sequences API
  slug: apollo-enrich-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-sequences-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apollo Enrich Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apollo.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apollo.io
provider_slug: apollo-enrich
scheme_count: 1
schemes:
- description: 'Apollo authenticates every request with an API key passed in the `x-api-key` header (for example `x-api-key: YOUR_API_KEY`). Keys are generated in Apollo''s developer settings. Some endpoints - such as People Search and listing account users - require a key that has been marked as a master key. API access is gated by plan tier: programmatic access begins on the Professional plan.'
  in: header
  keyName: x-api-key
  name: apiKeyAuth
  sources:
  - openapi/apollo-enrich-openapi.yml
  - https://docs.apollo.io/reference/authentication
  - https://docs.apollo.io/docs/create-api-key
  type: apiKey
slug: apollo-enrich-authentication
source_filename: apollo-enrich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apollo-enrich-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  description: >-\n    Apollo authenticates every request with an API key passed in the\n    `x-api-key` header (for example `x-api-key: YOUR_API_KEY`). Keys are\n    generated in Apollo's developer settings. Some endpoints - such as People\n    Search and listing account users - require a key that has been marked as a\n    master key. API access is gated by plan tier: programmatic access begins on\n    the Professional plan.\n  sources:\n  - openapi/apollo-enrich-openapi.yml\n  - https://docs.apollo.io/reference/authentication\n  - https://docs.apollo.io/docs/create-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/authentication/apollo-enrich-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Contact Discovery
- Data Enrichment
- Sales Intelligence
- B2B Data
- Prospecting
- Web Intelligence
- Lead Generation
- People Search
---
