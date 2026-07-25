---
api_key_in:
- header
api_specs:
- filename: pinecone-api-keys-api-openapi.yml
  format: yaml
  label: Pinecone API Keys API
  slug: pinecone-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-api-keys-api-openapi.yml
- filename: pinecone-bulk-operations-api-openapi.yml
  format: yaml
  label: Pinecone Bulk Operations API
  slug: pinecone-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-bulk-operations-api-openapi.yml
- filename: pinecone-inference-api-openapi.yml
  format: yaml
  label: Pinecone Inference API
  slug: pinecone-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-inference-api-openapi.yml
- filename: pinecone-manage-assistants-api-openapi.yml
  format: yaml
  label: Pinecone Manage Assistants API
  slug: pinecone-manage-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-manage-assistants-api-openapi.yml
- filename: pinecone-manage-indexes-api-openapi.yml
  format: yaml
  label: Pinecone Manage Indexes API
  slug: pinecone-manage-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-manage-indexes-api-openapi.yml
- filename: pinecone-namespace-operations-api-openapi.yml
  format: yaml
  label: Pinecone Namespace Operations API
  slug: pinecone-namespace-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-namespace-operations-api-openapi.yml
- filename: pinecone-organizations-api-openapi.yml
  format: yaml
  label: Pinecone Organizations API
  slug: pinecone-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-organizations-api-openapi.yml
- filename: pinecone-projects-api-openapi.yml
  format: yaml
  label: Pinecone Projects API
  slug: pinecone-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-projects-api-openapi.yml
- filename: pinecone-vector-operations-api-openapi.yml
  format: yaml
  label: Pinecone Vector Operations API
  slug: pinecone-vector-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-vector-operations-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinecone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinecone secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pinecone
provider_slug: pinecone
scheme_count: 2
schemes:
- description: An [access token](https://docs.pinecone.io/guides/organizations/manage-service-accounts#retrieve-an-access-token) must be provided in the `Authorization` header using the `Bearer` scheme.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pinecone-admin-openapi.yaml
  type: http
- description: Pinecone API Key
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/pinecone-assistant-control-openapi.yaml
  - openapi/pinecone-assistant-data-openapi.yaml
  - openapi/pinecone-db-control-openapi.yaml
  - openapi/pinecone-db-data-openapi.yaml
  - openapi/pinecone-inference-openapi.yaml
  type: apiKey
slug: pinecone-authentication
source_filename: pinecone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinecone-admin-openapi.yaml, openapi/pinecone-assistant-control-openapi.yaml,\n  openapi/pinecone-assistant-data-openapi.yaml, openapi/pinecone-db-control-openapi.yaml, openapi/pinecone-db-data-openapi.yaml,\n  openapi/pinecone-inference-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: An [access token](https://docs.pinecone.io/guides/organizations/manage-service-accounts#retrieve-an-access-token)\n    must be provided in the `Authorization` header using the `Bearer` scheme.\n  sources:\n  - openapi/pinecone-admin-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Pinecone API Key\n  sources:\n  - openapi/pinecone-assistant-control-openapi.yaml\n  - openapi/pinecone-assistant-data-openapi.yaml\n  - openapi/pinecone-db-control-openapi.yaml\n  - openapi/pinecone-db-data-openapi.yaml\n\
  \  - openapi/pinecone-inference-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/authentication/pinecone-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Vector Databases
- AI
- Embeddings
- RAG
---
