---
api_key_in: []
api_specs:
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instances API
  slug: instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instance Types & Availability API
  slug: instance-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Images & Startup Scripts API
  slug: images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch SSH Keys API
  slug: ssh-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Volumes API
  slug: volumes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Serverless Inference & Containers API
  slug: serverless-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Balance API
  slug: balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datacrunch Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataCrunch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataCrunch
provider_slug: datacrunch
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token obtained from POST /oauth2/token via the OAuth 2.0 Client Credentials grant.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datacrunch-openapi.yml
  type: http
slug: datacrunch-authentication
source_filename: datacrunch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datacrunch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token obtained from POST /oauth2/token via the OAuth 2.0 Client\n    Credentials grant.\n  sources:\n  - openapi/datacrunch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/authentication/datacrunch-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU Cloud
- Infrastructure
- Compute
- Inference
- Serverless
- Europe
---
