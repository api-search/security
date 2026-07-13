---
api_key_in:
- header
api_specs:
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Instances API
  slug: jarvislabs-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs GPU Types API
  slug: jarvislabs-gpu-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Templates API
  slug: jarvislabs-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Inference & Deploy API
  slug: jarvislabs-inference-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs SDK & CLI
  slug: jarvislabs-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jarvislabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: JarvisLabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JarvisLabs
provider_slug: jarvislabs
scheme_count: 1
schemes:
- description: API token generated at https://jarvislabs.ai/settings/api-keys. In the SDK this is set via jarvisclient.token; the CLI stores it via `jl setup`.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/jarvislabs-openapi.yml
  type: apiKey
slug: jarvislabs-authentication
source_filename: jarvislabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jarvislabs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token generated at https://jarvislabs.ai/settings/api-keys. In the SDK this\n    is set via jarvisclient.token; the CLI stores it via `jl setup`.\n  sources:\n  - openapi/jarvislabs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/authentication/jarvislabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- GPU
- Cloud
- Infrastructure
- Compute
---
