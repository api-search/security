---
api_key_in: []
api_specs:
- filename: vectorize-io-ai-platform-connectors-api-openapi.yml
  format: yaml
  label: Vectorize AI Platform Connectors API
  slug: vectorize-io-ai-platform-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-ai-platform-connectors-api-openapi.yml
- filename: vectorize-io-destination-connectors-api-openapi.yml
  format: yaml
  label: Vectorize Destination Connectors API
  slug: vectorize-io-destination-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-destination-connectors-api-openapi.yml
- filename: vectorize-io-extraction-api-openapi.yml
  format: yaml
  label: Vectorize Extraction API
  slug: vectorize-io-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-extraction-api-openapi.yml
- filename: vectorize-io-files-api-openapi.yml
  format: yaml
  label: Vectorize Files API
  slug: vectorize-io-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-files-api-openapi.yml
- filename: vectorize-io-pipelines-api-openapi.yml
  format: yaml
  label: Vectorize Pipelines API
  slug: vectorize-io-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-pipelines-api-openapi.yml
- filename: vectorize-io-source-connectors-api-openapi.yml
  format: yaml
  label: Vectorize Source Connectors API
  slug: vectorize-io-source-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-source-connectors-api-openapi.yml
- filename: vectorize-io-uploads-api-openapi.yml
  format: yaml
  label: Vectorize Uploads API
  slug: vectorize-io-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-uploads-api-openapi.yml
- filename: vectorize-io-workspaces-api-openapi.yml
  format: yaml
  label: Vectorize Workspaces API
  slug: vectorize-io-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vectorize Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vectorize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vectorize
provider_slug: vectorize-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Vectorize API access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vectorize-io-openapi.yml
  type: http
slug: vectorize-io-authentication
source_filename: vectorize-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vectorize-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Vectorize API access token passed as a Bearer token.\n  sources:\n  - openapi/vectorize-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/authentication/vectorize-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- RAG
- Vectorization
- Embeddings
- Retrieval
- Vector Database
---
