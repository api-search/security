---
api_key_in: []
api_specs:
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Link Search API
  slug: cj-affiliate-link-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Advertiser Lookup API
  slug: cj-affiliate-advertiser-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Publisher Lookup API
  slug: cj-affiliate-publisher-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Product Search (Legacy) API
  slug: cj-affiliate-product-search-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cj Affiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CJ Affiliate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CJ Affiliate
provider_slug: cj-affiliate
scheme_count: 1
schemes:
- description: 'Personal access token created in the CJ developer portal at https://developers.cj.com/account/personal-access-tokens and sent as ''Authorization: Bearer <token>''.'
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/cj-affiliate-openapi.yml
  type: http
slug: cj-affiliate-authentication
source_filename: cj-affiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cj-affiliate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: 'Personal access token created in the CJ developer portal at https://developers.cj.com/account/personal-access-tokens\n    and sent as ''Authorization: Bearer <token>''.'\n  sources:\n  - openapi/cj-affiliate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/authentication/cj-affiliate-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Affiliate Network
- Commission
- Product Search
- Publisher
- Advertiser
- GraphQL
- Ecommerce
---
