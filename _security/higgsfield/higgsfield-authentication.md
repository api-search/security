---
api_key_in:
- header
api_specs:
- filename: higgsfield-openapi-original.json
  format: json
  label: Higgsfield API
  slug: higgsfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/higgsfield/refs/heads/main/openapi/higgsfield-openapi-original.json
auth_types:
- http
description: 'The Higgsfield API authenticates with an API key and secret issued from the Higgsfield Cloud dashboard (cloud.higgsfield.ai). Credentials are sent on the Authorization header using the custom "Key" scheme: "Authorization: Key {api_key}:{api_key_secret}". There is no OAuth 2.0 / OIDC scope surface on the REST API (OAuth is used only for the remote MCP server). The OpenAPI document does not declare securitySchemes; this profile is captured from the developer docs.'
kind: authentication
layout: security
method: searched
name: Higgsfield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Higgsfield secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Higgsfield
provider_slug: higgsfield
scheme_count: 1
schemes:
- description: Custom Authorization scheme. The value is the literal word "Key" followed by the API key and secret joined with a colon. Generate credentials in the Higgsfield Cloud dashboard.
  format: Key {api_key}:{api_key_secret}
  header: Authorization
  in: header
  name: HiggsfieldKey
  scheme: Key
  sources:
  - https://docs.higgsfield.ai/docs/how-to/introduction
  type: http
slug: higgsfield-authentication
source_filename: higgsfield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.higgsfield.ai/docs/how-to/introduction + https://docs.higgsfield.ai/docs/how-to/sdk\ndocs: https://docs.higgsfield.ai/docs/how-to/introduction\ndescription: >-\n  The Higgsfield API authenticates with an API key and secret issued from the\n  Higgsfield Cloud dashboard (cloud.higgsfield.ai). Credentials are sent on the\n  Authorization header using the custom \"Key\" scheme:\n  \"Authorization: Key {api_key}:{api_key_secret}\". There is no OAuth 2.0 / OIDC\n  scope surface on the REST API (OAuth is used only for the remote MCP server).\n  The OpenAPI document does not declare securitySchemes; this profile is\n  captured from the developer docs.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: HiggsfieldKey\n  type: http\n  scheme: Key\n  in: header\n  header: Authorization\n  format: \"Key {api_key}:{api_key_secret}\"\n  description: >-\n    Custom Authorization scheme.\
  \ The value is the literal word \"Key\" followed by\n    the API key and secret joined with a colon. Generate credentials in the\n    Higgsfield Cloud dashboard.\n  sources:\n  - https://docs.higgsfield.ai/docs/how-to/introduction\ncredentials:\n  dashboard: https://cloud.higgsfield.ai/\n  sdk_env_vars:\n  - HF_KEY  # \"your-api-key:your-api-secret\"\n  - HF_API_KEY\n  - HF_API_SECRET\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higgsfield/refs/heads/main/authentication/higgsfield-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Generative AI
- Video Generation
- Image Generation
- Machine Learning
- Media
- Content Creation
- Developer API
---
