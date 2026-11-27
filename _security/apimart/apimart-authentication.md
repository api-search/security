---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: APIMart Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIMart declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: APIMart
provider_slug: apimart
scheme_count: 1
schemes:
- description: API keys are created on the API Key Management page (https://apimart.ai/keys). The docs recommend different keys per environment (development, testing, production), rotating keys regularly and regenerating a leaked key in the dashboard.
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  type: http
slug: apimart-authentication
source_filename: apimart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.apimart.ai/en/quickstart.md\ndocs: https://docs.apimart.ai/en/quickstart.md\nsee_also:\n- https://docs.apimart.ai/en/faqs/security-configuration.md\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  description: API keys are created on the API Key Management page (https://apimart.ai/keys). The docs recommend different keys per environment (development, testing, production), rotating keys regularly and regenerating a leaked key in the dashboard.\noauth2: false\nnote: The OpenAPI served at docs.apimart.ai/api-reference/openapi.json is the Mintlify \"OpenAPI Plant Store\" sample, not an APIMart contract, so no securitySchemes were derived from it.\n"
source_yaml_url: https://artifacts.apis.io/apimart/authentication/apimart-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Image Generation
- Video Generation
- OpenAI-Compatible
- Text-to-Speech
---
