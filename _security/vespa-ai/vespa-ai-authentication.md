---
api_key_in: []
api_specs:
- filename: vespa-query-api-openapi.yml
  format: yaml
  label: Vespa Query API
  slug: vespa-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/openapi/vespa-query-api-openapi.yml
- filename: vespa-document-api-openapi.yml
  format: yaml
  label: Vespa Document API
  slug: vespa-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/openapi/vespa-document-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vespa Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vespa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vespa
provider_slug: vespa-ai
scheme_count: 1
schemes:
- description: Vespa Cloud endpoints typically use mTLS with a client data-plane certificate.
  name: mtls
  scheme: bearer
  sources:
  - openapi/vespa-query-api-openapi.yml
  type: http
slug: vespa-ai-authentication
source_filename: vespa-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vespa-query-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: mtls\n  type: http\n  scheme: bearer\n  description: Vespa Cloud endpoints typically use mTLS with a client data-plane certificate.\n  sources:\n  - openapi/vespa-query-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/authentication/vespa-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Search
- Vector Database
- Big Data
- Machine Learning
- Semantic Search
- Retrieval Augmented Generation
- Open Source
- Tensor
- Recommendations
---
