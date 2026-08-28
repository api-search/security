---
api_key_in:
- header
api_specs:
- filename: nexgen-cloud-hyperstack-openapi.json
  format: json
  label: Hyperstack API
  slug: nexgen-cloud-hyperstack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/openapi/nexgen-cloud-hyperstack-openapi.json
- filename: nexgen-cloud-ai-studio-openapi.json
  format: json
  label: Hyperstack AI Studio API
  slug: nexgen-cloud-ai-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/openapi/nexgen-cloud-ai-studio-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nexgen Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: NexGen Cloud secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NexGen Cloud
provider_slug: nexgen-cloud
scheme_count: 2
schemes:
- description: 'API-key authentication. Pass your API key as the `api_key` header value (e.g., `api_key: YOUR_API_KEY`, no prefix). [Generate a key in the Hyperstack console](https://console.hyperstack.cloud/api-keys). The key is personal to your user account and works across every environment and region in your organization.'
  in: header
  name: apiKey
  parameter: api_key
  sources:
  - openapi/nexgen-cloud-ai-studio-openapi.json
  - openapi/nexgen-cloud-hyperstack-openapi.json
  - openapi/nexgen-cloud-infrahub-api-openapi.json
  type: apiKey
- description: Bearer Token
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/nexgen-cloud-infrahub-api-openapi.json
  type: apiKey
slug: nexgen-cloud-authentication
source_filename: nexgen-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/nexgen-cloud-ai-studio-openapi.json, openapi/nexgen-cloud-hyperstack-openapi.json,\n  openapi/nexgen-cloud-infrahub-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: 'API-key authentication. Pass your API key as the `api_key` header value (e.g.,\n    `api_key: YOUR_API_KEY`, no prefix). [Generate a key in the Hyperstack console](https://console.hyperstack.cloud/api-keys).\n    The key is personal to your user account and works across every environment and region in\n    your organization.'\n  sources:\n  - openapi/nexgen-cloud-ai-studio-openapi.json\n  - openapi/nexgen-cloud-hyperstack-openapi.json\n  - openapi/nexgen-cloud-infrahub-api-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer Token\n  sources:\n  - openapi/nexgen-cloud-infrahub-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/authentication/nexgen-cloud-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cloud
- GPU
- Artificial Intelligence
- Machine Learning
- Infrastructure
- Compute
- Kubernetes
- Storage
- Inference
- Virtual Machines
- Sovereign AI
---
