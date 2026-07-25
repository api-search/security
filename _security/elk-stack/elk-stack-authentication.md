---
api_key_in:
- header
api_specs:
- filename: elk-stack-cat-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Cat API
  slug: elk-stack-cat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-cat-api-openapi.yml
- filename: elk-stack-cluster-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Cluster API
  slug: elk-stack-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-cluster-api-openapi.yml
- filename: elk-stack-document-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Document API
  slug: elk-stack-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-document-api-openapi.yml
- filename: elk-stack-index-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Index API
  slug: elk-stack-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-index-api-openapi.yml
- filename: elk-stack-ingest-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Ingest API
  slug: elk-stack-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-ingest-api-openapi.yml
- filename: elk-stack-search-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Search API
  slug: elk-stack-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-search-api-openapi.yml
- filename: elk-stack-snapshot-api-openapi.yml
  format: yaml
  label: Elastic Stack (ELK Stack) Snapshot API
  slug: elk-stack-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/openapi/elk-stack-snapshot-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elk Stack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic Stack (ELK Stack) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic Stack (ELK Stack)
provider_slug: elk-stack
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elk-stack-openapi.yml
  type: http
- description: ApiKey <base64-encoded-id:api_key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elk-stack-openapi.yml
  type: apiKey
slug: elk-stack-authentication
source_filename: elk-stack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elk-stack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elk-stack-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: ApiKey <base64-encoded-id:api_key>\n  sources:\n  - openapi/elk-stack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/authentication/elk-stack-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Logging
- Monitoring
- Observability
- Search
---
