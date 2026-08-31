---
api_key_in: []
api_specs:
- filename: zoho-sign-accounts-api-openapi.yml
  format: yaml
  label: Zoho Sign Accounts API
  slug: zoho-sign-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/openapi/zoho-sign-accounts-api-openapi.yml
- filename: zoho-sign-requests-api-openapi.yml
  format: yaml
  label: Zoho Sign Requests API
  slug: zoho-sign-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/openapi/zoho-sign-requests-api-openapi.yml
- filename: zoho-sign-templates-api-openapi.yml
  format: yaml
  label: Zoho Sign Templates API
  slug: zoho-sign-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/openapi/zoho-sign-templates-api-openapi.yml
- filename: zoho-sign-users-api-openapi.yml
  format: yaml
  label: Zoho Sign Users API
  slug: zoho-sign-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/openapi/zoho-sign-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Sign Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Sign secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Sign
provider_slug: zoho-sign
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: zoho-sign-authentication
source_filename: zoho-sign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 3\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/authentication/zoho-sign-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Electronic Signatures
- eSignature
- Document-Management
- Digital Signatures
- Signature Workflows
- Templates
- Compliance
---
