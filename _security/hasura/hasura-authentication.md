---
api_key_in:
- header
api_specs:
- filename: hasura-asyncapi.yml
  format: yaml
  label: Hasura GraphQL API
  slug: hasura-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/asyncapi/hasura-asyncapi.yml
- filename: hasura-metadata-api-openapi.yml
  format: yaml
  label: Hasura Metadata API
  slug: hasura-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-metadata-api-openapi.yml
- filename: hasura-graphql-api-openapi.yml
  format: yaml
  label: Hasura Graphql API
  slug: hasura-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-graphql-api-openapi.yml
- filename: hasura-healthz-api-openapi.yml
  format: yaml
  label: Hasura Healthz API
  slug: hasura-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-healthz-api-openapi.yml
- filename: hasura-metadata-api-openapi.yml
  format: yaml
  label: Hasura Metadata API
  slug: hasura-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-metadata-api-openapi.yml
- filename: hasura-query-api-openapi.yml
  format: yaml
  label: Hasura Query API
  slug: hasura-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-query-api-openapi.yml
- filename: hasura-source-health-api-openapi.yml
  format: yaml
  label: Hasura Source Health API
  slug: hasura-source-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-source-health-api-openapi.yml
- filename: hasura-v1alpha1-api-openapi.yml
  format: yaml
  label: Hasura V1alpha1 API
  slug: hasura-v1alpha1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-v1alpha1-api-openapi.yml
- filename: hasura-v1beta1-api-openapi.yml
  format: yaml
  label: Hasura V1beta1 API
  slug: hasura-v1beta1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-v1beta1-api-openapi.yml
- filename: hasura-version-api-openapi.yml
  format: yaml
  label: Hasura Version API
  slug: hasura-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-version-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hasura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hasura secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hasura
provider_slug: hasura
scheme_count: 2
schemes:
- description: Admin secret configured via HASURA_GRAPHQL_ADMIN_SECRET.
  in: header
  name: adminSecret
  parameter: x-hasura-admin-secret
  sources:
  - openapi/hasura-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token, when JWT authentication is configured.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hasura-openapi.yml
  type: http
slug: hasura-authentication
source_filename: hasura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hasura-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: adminSecret\n  type: apiKey\n  in: header\n  parameter: x-hasura-admin-secret\n  description: Admin secret configured via HASURA_GRAPHQL_ADMIN_SECRET.\n  sources:\n  - openapi/hasura-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token, when JWT authentication is configured.\n  sources:\n  - openapi/hasura-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/authentication/hasura-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Access
- GraphQL
---
