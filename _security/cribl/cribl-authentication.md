---
api_key_in: []
api_specs:
- filename: cribl-cloud-api-openapi.yml
  format: yaml
  label: Cribl Cloud API
  slug: cribl-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-cloud-api-openapi.yml
- filename: cribl-stream-api-openapi.yml
  format: yaml
  label: Cribl Stream API
  slug: cribl-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-stream-api-openapi.yml
- filename: cribl-edge-api-openapi.yml
  format: yaml
  label: Cribl Edge API
  slug: cribl-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-edge-api-openapi.yml
- filename: cribl-search-api-openapi.yml
  format: yaml
  label: Cribl Search API
  slug: cribl-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-search-api-openapi.yml
- filename: cribl-lake-api-openapi.yml
  format: yaml
  label: Cribl Lake API
  slug: cribl-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-lake-api-openapi.yml
- filename: cribl-as-code-api-openapi.yml
  format: yaml
  label: Cribl As Code API
  slug: cribl-as-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/openapi/cribl-as-code-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cribl Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cribl secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cribl
provider_slug: cribl
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token obtained via OAuth 2.0 client credentials grant from https://login.cribl.cloud/oauth/token. Tokens expire after 24 hours (86400 seconds).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cribl-as-code-api-openapi.yml
  - openapi/cribl-cloud-api-openapi.yml
  - openapi/cribl-edge-api-openapi.yml
  - openapi/cribl-lake-api-openapi.yml
  - openapi/cribl-search-api-openapi.yml
  - openapi/cribl-stream-api-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow for Cribl Cloud management plane authentication.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://login.cribl.cloud/oauth/token
  name: oauth2
  sources:
  - openapi/cribl-as-code-api-openapi.yml
  - openapi/cribl-cloud-api-openapi.yml
  type: oauth2
slug: cribl-authentication
source_filename: cribl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cribl-as-code-api-openapi.yml, openapi/cribl-cloud-api-openapi.yml, openapi/cribl-edge-api-openapi.yml,\n  openapi/cribl-lake-api-openapi.yml, openapi/cribl-search-api-openapi.yml, openapi/cribl-stream-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained via OAuth 2.0 client credentials grant from https://login.cribl.cloud/oauth/token.\n    Tokens expire after 24 hours (86400 seconds).\n  sources:\n  - openapi/cribl-as-code-api-openapi.yml\n  - openapi/cribl-cloud-api-openapi.yml\n  - openapi/cribl-edge-api-openapi.yml\n  - openapi/cribl-lake-api-openapi.yml\n  - openapi/cribl-search-api-openapi.yml\n  - openapi/cribl-stream-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.cribl.cloud/oauth/token\n\
  \    scopes: 0\n  description: OAuth 2.0 client credentials flow for Cribl Cloud management plane authentication.\n  sources:\n  - openapi/cribl-as-code-api-openapi.yml\n  - openapi/cribl-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/authentication/cribl-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
---
