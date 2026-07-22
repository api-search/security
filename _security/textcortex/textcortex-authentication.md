---
api_key_in: []
api_specs:
- filename: textcortex-openapi.json
  format: json
  label: TextCortex API
  slug: textcortex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textcortex/refs/heads/main/openapi/textcortex-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Textcortex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Textcortex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Textcortex
provider_slug: textcortex
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'Send `Authorization: Bearer <api_key>`.'
  how_to_obtain: TextCortex dashboard -> Settings -> API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/textcortex-openapi.json
  type: http
slug: textcortex-authentication
source_filename: textcortex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/textcortex-openapi.json\ndocs: https://docs.textcortex.com/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  notes: >-\n    Single auth model. The public REST API authenticates with a per-account API key\n    sent as an HTTP Bearer token in the Authorization header. Generate the key from\n    the TextCortex dashboard Settings. There is no OAuth flow for the REST API; a\n    separate OIDC discovery document (well-known/textcortex-openid-configuration.json)\n    covers account/dashboard login only (scopes openid/email/profile).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Send `Authorization: Bearer <api_key>`.'\n  how_to_obtain: TextCortex dashboard -> Settings -> API Key\n  sources:\n  - openapi/textcortex-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textcortex/refs/heads/main/authentication/textcortex-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Text Generation
- Large Language Models
- Chat Completions
- OpenAI-Compatible
- Content Generation
- Developer Tools
---
