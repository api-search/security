---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inboxacademy-io-learning-api-openapi.yml
  format: yaml
  label: Inbox Academy Learning API
  slug: inboxacademy-io-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxacademy-io/openapi/inboxacademy-io-learning-api-openapi.yml
auth_types: []
description: Authentication methods for Inbox Academy API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Inbox Academy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inbox Academy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Inbox Academy
provider_slug: inboxacademy-io
scheme_count: 2
schemes:
- evidence: 'Using it Whatever you are connecting sends the key as a bearer token: Authorization: Bearer elk_...'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://inboxacademy.io/mcp/oauth/authorize
  evidence: 'grant_types_supported": ["authorization_code", "refresh_token"]'
  flows:
  - authorization_code
  name: OAuth2
  scopes:
  - content:read
  - content:write
  type: oauth2
slug: inboxacademy-io-authentication
source_filename: inboxacademy-io-authentication.yml
source_heading: Authentication Profile
source_url: https://inboxacademy.io/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inboxacademy.io/.well-known/oauth-authorization-server\nsources:\n- https://inboxacademy.io/.well-known/oauth-authorization-server\n- https://inboxacademy.io/guide/create-and-revoke-an-api-key/\n- https://inboxacademy.io/solutions/employee-onboarding/\n- https://inboxacademy.io/solutions/customer-onboarding/\ndescription: Authentication methods for Inbox Academy API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Using it Whatever you are connecting sends the key as a bearer token: Authorization: Bearer elk_...'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth2\n  evidence: 'grant_types_supported\": [\"authorization_code\", \"refresh_token\"]'\n  flows:\n  - authorization_code\n  authorize_url: https://inboxacademy.io/mcp/oauth/authorize\n  scopes:\n  - content:read\n  - content:write\ndocs: https://inboxacademy.io/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/inboxacademy-io/authentication/inboxacademy-io-authentication.yml
summary_line: 2 schemes
tags:
- Email
- Onboarding
- Training
- Education
- Software-as-a-Service
- Platform
---
