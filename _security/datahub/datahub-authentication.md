---
api_key_in: []
api_specs:
- filename: datahub-openapi-openapi.yml
  format: yaml
  label: DataHub OpenAPI
  slug: datahub-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/openapi/datahub-openapi-openapi.yml
- filename: datahub-actions-asyncapi.yml
  format: yaml
  label: DataHub Actions Framework
  slug: datahub-actions-framework
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/asyncapi/datahub-actions-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datahub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataHub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataHub
provider_slug: datahub
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: DataHub personal access token or session token. Generate tokens via the DataHub settings panel or programmatically using the token management API. Pass the token in the Authorization header as Bearer <token>.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datahub-openapi-openapi.yml
  type: http
slug: datahub-authentication
source_filename: datahub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datahub-openapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: DataHub personal access token or session token. Generate tokens via the DataHub\n    settings panel or programmatically using the token management API. Pass the token in the\n    Authorization header as Bearer <token>.\n  sources:\n  - openapi/datahub-openapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/authentication/datahub-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Catalog
- Data Discovery
- Data Governance
- Data Lineage
- Metadata
---
