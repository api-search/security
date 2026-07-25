---
api_key_in: []
api_specs:
- filename: sailpoint-access-profiles-api-openapi.yml
  format: yaml
  label: SailPoint Access Profiles API
  slug: sailpoint-access-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/openapi/sailpoint-access-profiles-api-openapi.yml
- filename: sailpoint-certifications-api-openapi.yml
  format: yaml
  label: SailPoint Certifications API
  slug: sailpoint-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/openapi/sailpoint-certifications-api-openapi.yml
- filename: sailpoint-identities-api-openapi.yml
  format: yaml
  label: SailPoint Identities API
  slug: sailpoint-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/openapi/sailpoint-identities-api-openapi.yml
- filename: sailpoint-roles-api-openapi.yml
  format: yaml
  label: SailPoint Roles API
  slug: sailpoint-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/openapi/sailpoint-roles-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sailpoint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: SailPoint secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: SailPoint
provider_slug: sailpoint
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication. Use client credentials or authorization code flow to obtain access tokens.
  flows:
  - flow: clientCredentials
    scopes: 11
    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token
  - authorizationUrl: https://{tenant}.identitynow.com/oauth/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token
  name: oauth2
  sources:
  - openapi/identity-security-cloud-v3.yml
  type: oauth2
- bearerFormat: JWT
  description: Personal access token (PAT) authentication. Generate a PAT in Identity Security Cloud and use it as a bearer token.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/identity-security-cloud-v3.yml
  type: http
slug: sailpoint-authentication
source_filename: sailpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/identity-security-cloud-v3.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token\n    scopes: 11\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.identitynow.com/oauth/authorize\n    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token\n    scopes: 11\n  description: OAuth 2.0 authentication. Use client credentials or authorization code flow to\n    obtain access tokens.\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Personal access token (PAT) authentication. Generate a PAT in Identity Security\n    Cloud and use it as a bearer token.\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/authentication/sailpoint-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Access Governance
- Compliance
- IAM
- Identity Management
- Identity Security
- Security
---
