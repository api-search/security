---
api_key_in: []
api_specs:
- filename: prove-auth-api-openapi.yml
  format: yaml
  label: Prove Auth API
  slug: prove-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-auth-api-openapi.yml
- filename: prove-authentication-api-openapi.yml
  format: yaml
  label: Prove Authentication API
  slug: prove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-authentication-api-openapi.yml
- filename: prove-domain-api-openapi.yml
  format: yaml
  label: Prove Domain API
  slug: prove-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-domain-api-openapi.yml
- filename: prove-identity-api-openapi.yml
  format: yaml
  label: Prove Identity API
  slug: prove-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-api-openapi.yml
- filename: prove-identity-verification-api-openapi.yml
  format: yaml
  label: Prove Identity Verification API
  slug: prove-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-verification-api-openapi.yml
- filename: prove-pre-fill-api-openapi.yml
  format: yaml
  label: Prove Pre-Fill API
  slug: prove-pre-fill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-pre-fill-api-openapi.yml
- filename: prove-trust-score-api-openapi.yml
  format: yaml
  label: Prove Trust Score API
  slug: prove-trust-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-trust-score-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Prove Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Prove secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Prove
provider_slug: prove
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 client-credentials Bearer access token obtained from POST /token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prove-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  sources:
  - openapi/prove-openapi.yml
  type: oauth2
slug: prove-authentication
source_filename: prove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prove-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 client-credentials Bearer access token obtained from POST /token.\n  sources:\n  - openapi/prove-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n    scopes: 0\n  sources:\n  - openapi/prove-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/authentication/prove-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity Verification
- Authentication
- Phone Intelligence
- KYC
- Fraud Prevention
---
