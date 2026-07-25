---
api_key_in: []
api_specs:
- filename: datacrunch-balance-api-openapi.yml
  format: yaml
  label: DataCrunch Balance API
  slug: datacrunch-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-balance-api-openapi.yml
- filename: datacrunch-images-api-openapi.yml
  format: yaml
  label: DataCrunch Images API
  slug: datacrunch-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-images-api-openapi.yml
- filename: datacrunch-instance-availability-api-openapi.yml
  format: yaml
  label: DataCrunch Instance Availability API
  slug: datacrunch-instance-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-instance-availability-api-openapi.yml
- filename: datacrunch-instance-types-api-openapi.yml
  format: yaml
  label: DataCrunch Instance Types API
  slug: datacrunch-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-instance-types-api-openapi.yml
- filename: datacrunch-instances-api-openapi.yml
  format: yaml
  label: DataCrunch Instances API
  slug: datacrunch-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-instances-api-openapi.yml
- filename: datacrunch-locations-api-openapi.yml
  format: yaml
  label: DataCrunch Locations API
  slug: datacrunch-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-locations-api-openapi.yml
- filename: datacrunch-oauth-api-openapi.yml
  format: yaml
  label: DataCrunch OAuth API
  slug: datacrunch-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-oauth-api-openapi.yml
- filename: datacrunch-serverless-containers-api-openapi.yml
  format: yaml
  label: DataCrunch Serverless Containers API
  slug: datacrunch-serverless-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-serverless-containers-api-openapi.yml
- filename: datacrunch-ssh-keys-api-openapi.yml
  format: yaml
  label: DataCrunch SSH Keys API
  slug: datacrunch-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-ssh-keys-api-openapi.yml
- filename: datacrunch-startup-scripts-api-openapi.yml
  format: yaml
  label: DataCrunch Startup Scripts API
  slug: datacrunch-startup-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-startup-scripts-api-openapi.yml
- filename: datacrunch-volumes-api-openapi.yml
  format: yaml
  label: DataCrunch Volumes API
  slug: datacrunch-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-volumes-api-openapi.yml
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
