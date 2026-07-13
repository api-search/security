---
api_key_in: []
api_specs:
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: paragon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Integrations API
  slug: paragon-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Users API
  slug: paragon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: paragon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: paragon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: paragon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Managed Sync API
  slug: paragon-managed-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Permissions API
  slug: paragon-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Events and Webhooks API
  slug: paragon-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Useparagon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paragon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paragon
provider_slug: useparagon
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'A Paragon User Token: an RS256-signed JWT whose subject identifies the end user. Sign it with the private signing key from Settings > SDK Setup in the Paragon dashboard; Paragon verifies it with the matching public key.'
  name: ParagonUserToken
  scheme: bearer
  sources:
  - openapi/useparagon-openapi.yml
  type: http
slug: useparagon-authentication
source_filename: useparagon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/useparagon-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ParagonUserToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'A Paragon User Token: an RS256-signed JWT whose subject identifies the end user.\n    Sign it with the private signing key from Settings > SDK Setup in the Paragon dashboard;\n    Paragon verifies it with the matching public key.'\n  sources:\n  - openapi/useparagon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/authentication/useparagon-authentication.yml
summary_line: http · 1 scheme
tags:
- Integration
- iPaaS
- Embedded Integrations
- Workflows
- ActionKit
- Managed Sync
- AI Agents
---
