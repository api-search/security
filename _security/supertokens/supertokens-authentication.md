---
api_key_in:
- header
api_specs:
- filename: supertokens-email-password-api-openapi.yml
  format: yaml
  label: SuperTokens Email Password API
  slug: supertokens-email-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-email-password-api-openapi.yml
- filename: supertokens-email-verification-api-openapi.yml
  format: yaml
  label: SuperTokens Email Verification API
  slug: supertokens-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-email-verification-api-openapi.yml
- filename: supertokens-health-api-openapi.yml
  format: yaml
  label: SuperTokens Health API
  slug: supertokens-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-health-api-openapi.yml
- filename: supertokens-multi-tenancy-api-openapi.yml
  format: yaml
  label: SuperTokens Multi Tenancy API
  slug: supertokens-multi-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-multi-tenancy-api-openapi.yml
- filename: supertokens-passwordless-api-openapi.yml
  format: yaml
  label: SuperTokens Passwordless API
  slug: supertokens-passwordless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-passwordless-api-openapi.yml
- filename: supertokens-sessions-api-openapi.yml
  format: yaml
  label: SuperTokens Sessions API
  slug: supertokens-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-sessions-api-openapi.yml
- filename: supertokens-third-party-api-openapi.yml
  format: yaml
  label: SuperTokens Third Party API
  slug: supertokens-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-third-party-api-openapi.yml
- filename: supertokens-user-metadata-api-openapi.yml
  format: yaml
  label: SuperTokens User Metadata API
  slug: supertokens-user-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-user-metadata-api-openapi.yml
- filename: supertokens-user-roles-api-openapi.yml
  format: yaml
  label: SuperTokens User Roles API
  slug: supertokens-user-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-user-roles-api-openapi.yml
- filename: supertokens-users-api-openapi.yml
  format: yaml
  label: SuperTokens Users API
  slug: supertokens-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supertokens/refs/heads/main/openapi/supertokens-users-api-openapi.yml
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
- Open-Source
- Session Management
- Social Login
- Passwordless
- Identity
- Authorization
- Multi-Tenancy
- Node.js
- Self-Hosted
---
