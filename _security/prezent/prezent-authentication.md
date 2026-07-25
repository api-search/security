---
api_key_in: []
api_specs:
- filename: prezent-audiences-api-openapi.yml
  format: yaml
  label: Prezent Audiences API
  slug: prezent-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-audiences-api-openapi.yml
- filename: prezent-autogenerator-api-openapi.yml
  format: yaml
  label: Prezent AutoGenerator API
  slug: prezent-autogenerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-autogenerator-api-openapi.yml
- filename: prezent-file-access-api-openapi.yml
  format: yaml
  label: Prezent File Access API
  slug: prezent-file-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-file-access-api-openapi.yml
- filename: prezent-health-api-openapi.yml
  format: yaml
  label: Prezent Health API
  slug: prezent-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-health-api-openapi.yml
- filename: prezent-streaming-api-openapi.yml
  format: yaml
  label: Prezent Streaming API
  slug: prezent-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-streaming-api-openapi.yml
- filename: prezent-template-converter-api-openapi.yml
  format: yaml
  label: Prezent Template Converter API
  slug: prezent-template-converter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-template-converter-api-openapi.yml
- filename: prezent-themes-api-openapi.yml
  format: yaml
  label: Prezent Themes API
  slug: prezent-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-themes-api-openapi.yml
- filename: prezent-upload-api-openapi.yml
  format: yaml
  label: Prezent Upload API
  slug: prezent-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-upload-api-openapi.yml
- filename: prezent-webhooks-api-openapi.yml
  format: yaml
  label: Prezent Webhooks API
  slug: prezent-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prezent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prezent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prezent
provider_slug: prezent
scheme_count: 1
schemes:
- bearerFormat: opaque
  description: 'Bearer token authentication. Supply the API key issued by

    Customer Success as `Authorization: Bearer <api_key>`. The API

    does NOT accept the AWS `x-api-key` header. Keys may have an

    expiry date; expired keys return `401 EXPIRED_API_KEY`. Keys are

    scoped to specific paths; calling an unauthorised path returns

    `404 ENDPOINT_NOT_FOUND`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/prezent-openapi-original.yml
  type: http
slug: prezent-authentication
source_filename: prezent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prezent-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: |-\n    Bearer token authentication. Supply the API key issued by\n    Customer Success as `Authorization: Bearer <api_key>`. The API\n    does NOT accept the AWS `x-api-key` header. Keys may have an\n    expiry date; expired keys return `401 EXPIRED_API_KEY`. Keys are\n    scoped to specific paths; calling an unauthorised path returns\n    `404 ENDPOINT_NOT_FOUND`.\n  sources:\n  - openapi/prezent-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/authentication/prezent-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Presentations
- Generative AI
- AI Agents
- Life Sciences
- Content Generation
- Enterprise
- MCP
- Productivity
---
