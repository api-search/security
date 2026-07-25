---
api_key_in: []
api_specs:
- filename: useparagon-actionkit-api-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: useparagon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-actionkit-api-openapi.yml
- filename: useparagon-connect-api-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: useparagon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-connect-api-openapi.yml
- filename: useparagon-integrations-api-openapi.yml
  format: yaml
  label: Paragon Integrations API
  slug: useparagon-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-integrations-api-openapi.yml
- filename: useparagon-managed-sync-api-openapi.yml
  format: yaml
  label: Paragon Managed Sync API
  slug: useparagon-managed-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-managed-sync-api-openapi.yml
- filename: useparagon-permissions-api-openapi.yml
  format: yaml
  label: Paragon Permissions API
  slug: useparagon-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-permissions-api-openapi.yml
- filename: useparagon-proxy-api-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: useparagon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-proxy-api-openapi.yml
- filename: useparagon-users-api-openapi.yml
  format: yaml
  label: Paragon Users API
  slug: useparagon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-users-api-openapi.yml
- filename: useparagon-workflows-api-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: useparagon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-workflows-api-openapi.yml
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
