---
anonymous_access: false
api_key_in: []
api_specs:
- filename: secure-flows-com-ai-optional-api-openapi.yml
  format: yaml
  label: secure-flows-com AI Optional API
  slug: secure-flows-com-ai-optional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-ai-optional-api-openapi.yml
- filename: secure-flows-com-ai-safe-api-openapi.yml
  format: yaml
  label: secure-flows-com AI Safe API
  slug: secure-flows-com-ai-safe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-ai-safe-api-openapi.yml
- filename: secure-flows-com-applications-api-openapi.yml
  format: yaml
  label: secure-flows-com Applications API
  slug: secure-flows-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-applications-api-openapi.yml
- filename: secure-flows-com-audit-api-openapi.yml
  format: yaml
  label: secure-flows-com Audit API
  slug: secure-flows-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-audit-api-openapi.yml
- filename: secure-flows-com-hosted-ui-api-openapi.yml
  format: yaml
  label: secure-flows-com Hosted UI API
  slug: secure-flows-com-hosted-ui-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-hosted-ui-api-openapi.yml
- filename: secure-flows-com-human-only-api-openapi.yml
  format: yaml
  label: secure-flows-com Human Only API
  slug: secure-flows-com-human-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-human-only-api-openapi.yml
- filename: secure-flows-com-users-api-openapi.yml
  format: yaml
  label: secure-flows-com Users API
  slug: secure-flows-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secure-flows-com/openapi/secure-flows-com-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Secure Flows Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: secure-flows-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: secure-flows-com
provider_slug: secure-flows-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Firebase ID token (POST /sessions, POST /sessions/get-or-create, POST /sessions/renew/{sessionToken})
  name: firebaseBearerAuth
  scheme: bearer
  type: http
- bearerFormat: JWT
  description: Session JWT from POST /sessions or POST /sessions/renew/{sessionToken}
  name: sessionBearerAuth
  scheme: bearer
  type: http
slug: secure-flows-com-authentication
source_filename: secure-flows-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/secure-flows-session-api.yaml\nschemes:\n  - name: firebaseBearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: 'Firebase ID token (POST /sessions, POST /sessions/get-or-create, POST /sessions/renew/{sessionToken})'\n  - name: sessionBearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: 'Session JWT from POST /sessions or POST /sessions/renew/{sessionToken}'\n"
source_yaml_url: https://artifacts.apis.io/secure-flows-com/authentication/secure-flows-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Data-Encryption
- No-code
- Authentication
---
