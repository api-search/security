---
api_key_in:
- header
api_specs:
- filename: supertokens-core-driver-interface-openapi.yml
  format: yaml
  label: SuperTokens Core Driver Interface
  slug: core-driver-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-core-driver-interface-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Supertokens Authentication
name_suffix: Authentication
oauth_flows: []
overview: SuperTokens secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SuperTokens
provider_slug: supertokens
scheme_count: 1
schemes:
- description: SuperTokens Core API key (configured in config.yaml or via environment variable)
  in: header
  name: ApiKeyAuth
  parameter: api-key
  sources:
  - openapi/supertokens-core-driver-interface-openapi.yml
  type: apiKey
slug: supertokens-authentication
source_filename: supertokens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/supertokens-core-driver-interface-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: SuperTokens Core API key (configured in config.yaml or via environment variable)\n  sources:\n  - openapi/supertokens-core-driver-interface-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/authentication/supertokens-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Open Source
- Session Management
- Social Login
- Passwordless
- Identity
- Authorization
- Multi-Tenancy
- Node.js
- Self-Hosted
---
