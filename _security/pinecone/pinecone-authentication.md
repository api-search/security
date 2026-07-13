---
api_key_in:
- header
api_specs:
- filename: pinecone-db-control-openapi.yaml
  format: yaml
  label: Pinecone Database Control API
  slug: pinecone-database-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-db-control-openapi.yaml
- filename: pinecone-db-data-openapi.yaml
  format: yaml
  label: Pinecone Database Data API
  slug: pinecone-database-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-db-data-openapi.yaml
- filename: pinecone-inference-openapi.yaml
  format: yaml
  label: Pinecone Inference API
  slug: pinecone-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-inference-openapi.yaml
- filename: pinecone-assistant-control-openapi.yaml
  format: yaml
  label: Pinecone Assistant Control API
  slug: pinecone-assistant-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-assistant-control-openapi.yaml
- filename: pinecone-assistant-data-openapi.yaml
  format: yaml
  label: Pinecone Assistant Data API
  slug: pinecone-assistant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-assistant-data-openapi.yaml
- filename: pinecone-admin-openapi.yaml
  format: yaml
  label: Pinecone Admin API
  slug: pinecone-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-admin-openapi.yaml
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
