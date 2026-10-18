---
anonymous_access: false
api_key_in: []
api_specs:
- filename: atlas-cloud-balance-api-openapi.yml
  format: yaml
  label: Atlas Cloud Balance API
  slug: atlas-cloud-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-balance-api-openapi.yml
- filename: atlas-cloud-completions-api-openapi.yml
  format: yaml
  label: Atlas Cloud Completions API
  slug: atlas-cloud-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-completions-api-openapi.yml
- filename: atlas-cloud-images-api-openapi.yml
  format: yaml
  label: Atlas Cloud Images API
  slug: atlas-cloud-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-images-api-openapi.yml
- filename: atlas-cloud-messages-api-openapi.yml
  format: yaml
  label: Atlas Cloud Messages API
  slug: atlas-cloud-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-messages-api-openapi.yml
- filename: atlas-cloud-model-api-openapi.yml
  format: yaml
  label: Atlas Cloud Model API
  slug: atlas-cloud-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-model-api-openapi.yml
- filename: atlas-cloud-model-costs-api-openapi.yml
  format: yaml
  label: Atlas Cloud Model Costs API
  slug: atlas-cloud-model-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-model-costs-api-openapi.yml
- filename: atlas-cloud-model-usage-api-openapi.yml
  format: yaml
  label: Atlas Cloud Model Usage API
  slug: atlas-cloud-model-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-model-usage-api-openapi.yml
- filename: atlas-cloud-v1beta-api-openapi.yml
  format: yaml
  label: Atlas Cloud V1Beta API
  slug: atlas-cloud-v1beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-v1beta-api-openapi.yml
- filename: atlas-cloud-webhooks-api-openapi.yml
  format: yaml
  label: Atlas Cloud Webhooks API
  slug: atlas-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-webhooks-api-openapi.yml
- filename: atlas-cloud-chat-completions-api-openapi.yml
  format: yaml
  label: Atlas Cloud Chat Completions API
  slug: atlas-cloud-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/openapi/atlas-cloud-chat-completions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Atlas Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atlas Cloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Atlas Cloud
provider_slug: atlas-cloud
scheme_count: 1
schemes:
- description: Include your API key in the Authorization header of every API request; keys are shown once at creation and can be rotated in the console.
  header: Authorization
  in: header
  name: API key
  scheme: bearer
  type: http
slug: atlas-cloud-authentication
source_filename: atlas-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Atlas Cloud authentication\ngenerated: '2026-10-13'\nmethod: searched\nsource: https://www.atlascloud.ai/docs/api-keys\ndocs: https://www.atlascloud.ai/docs/api-keys\nschemes:\n- type: http\n  scheme: bearer\n  name: API key\n  in: header\n  header: Authorization\n  description: Include your API key in the Authorization header of every API request;\n    keys are shown once at creation and can be rotated in the console.\nrbac: https://www.atlascloud.ai/docs/account/rbac\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas-cloud/refs/heads/main/authentication/atlas-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Model Routing
- Image Generation
- Video Generation
- Inference
- GPU Cloud
- MCP
---
