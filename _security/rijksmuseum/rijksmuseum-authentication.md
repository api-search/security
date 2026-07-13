---
api_key_in:
- query
api_specs:
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Search API
  slug: collection-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Details API
  slug: collection-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Image Tiles API
  slug: collection-image-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-user-sets-openapi.yml
  format: yaml
  label: Usersets API
  slug: usersets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-user-sets-openapi.yml
- filename: rijksmuseum-user-sets-openapi.yml
  format: yaml
  label: Userset Details API
  slug: userset-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-user-sets-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rijksmuseum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rijksmuseum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rijksmuseum
provider_slug: rijksmuseum
scheme_count: 1
schemes:
- description: 'Free API key issued on creating a Rijksstudio account at

    https://www.rijksmuseum.nl/en/rijksstudio. The key is available from the

    account''s advanced settings.'
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/rijksmuseum-collection-openapi.yml
  - openapi/rijksmuseum-user-sets-openapi.yml
  type: apiKey
slug: rijksmuseum-authentication
source_filename: rijksmuseum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rijksmuseum-collection-openapi.yml, openapi/rijksmuseum-user-sets-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: |-\n    Free API key issued on creating a Rijksstudio account at\n    https://www.rijksmuseum.nl/en/rijksstudio. The key is available from the\n    account's advanced settings.\n  sources:\n  - openapi/rijksmuseum-collection-openapi.yml\n  - openapi/rijksmuseum-user-sets-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/authentication/rijksmuseum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Art And Design
- Museums
- Cultural Heritage
- Open Data
- Linked Data
- OAI-PMH
- IIIF
- Dutch Heritage
- Public APIs
---
