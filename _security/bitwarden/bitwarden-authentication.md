---
api_key_in: []
api_specs:
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Members
  slug: public-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Groups
  slug: public-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Collections
  slug: public-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Policies
  slug: public-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Event Logs
  slug: public-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bitwarden Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bitwarden secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bitwarden
provider_slug: bitwarden
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://identity.bitwarden.com/connect/token
  name: OAuth2 Client Credentials
  sources:
  - openapi/bitwarden-public-swagger.json
  type: oauth2
slug: bitwarden-authentication
source_filename: bitwarden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitwarden-public-swagger.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2 Client Credentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.bitwarden.com/connect/token\n    scopes: 1\n  sources:\n  - openapi/bitwarden-public-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/authentication/bitwarden-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Security
- Password Manager
- Open Source
- Vault
- Identity
- SCIM
---
