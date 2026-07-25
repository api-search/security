---
api_key_in: []
api_specs:
- filename: marqo-documents-api-openapi.yml
  format: yaml
  label: Marqo Documents API
  slug: marqo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-documents-api-openapi.yml
- filename: marqo-embeddings-api-openapi.yml
  format: yaml
  label: Marqo Embeddings API
  slug: marqo-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-embeddings-api-openapi.yml
- filename: marqo-indexes-api-openapi.yml
  format: yaml
  label: Marqo Indexes API
  slug: marqo-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-indexes-api-openapi.yml
- filename: marqo-models-api-openapi.yml
  format: yaml
  label: Marqo Models API
  slug: marqo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-models-api-openapi.yml
- filename: marqo-recommendations-api-openapi.yml
  format: yaml
  label: Marqo Recommendations API
  slug: marqo-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-recommendations-api-openapi.yml
- filename: marqo-search-api-openapi.yml
  format: yaml
  label: Marqo Search API
  slug: marqo-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-search-api-openapi.yml
- filename: marqo-telemetry-api-openapi.yml
  format: yaml
  label: Marqo Telemetry API
  slug: marqo-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-telemetry-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Marqo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marqo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Marqo
provider_slug: marqo
scheme_count: 1
schemes:
- description: 'Marqo Cloud API key passed as `Authorization: Bearer {api_key}`.

    The open-source engine accepts unauthenticated requests by default.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/marqo-openapi.yml
  type: http
slug: marqo-authentication
source_filename: marqo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marqo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Marqo Cloud API key passed as `Authorization: Bearer {api_key}`.\n    The open-source engine accepts unauthenticated requests by default.\n  sources:\n  - openapi/marqo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/authentication/marqo-authentication.yml
summary_line: http · 1 scheme
tags:
- Vector Database
- Vector Search
- Multimodal
- Semantic Search
- Embeddings
- AI
- Machine Learning
- Open Source
- Ecommerce Search
---
