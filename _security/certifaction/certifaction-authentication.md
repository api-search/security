---
api_key_in:
- header
api_specs:
- filename: certifaction-local-api-openapi.yml
  format: yaml
  label: Certifaction Local API
  slug: certifaction-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-local-api-openapi.yml
- filename: certifaction-admin-api-openapi.yml
  format: yaml
  label: Certifaction Admin API
  slug: certifaction-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-admin-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Certifaction Authentication
name_suffix: Authentication
oauth_flows:
- oidc-external
overview: Certifaction secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the oidc-external flow(s).
provider_name: Certifaction
provider_slug: certifaction
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/certifaction-admin-api-openapi.yml
  - openapi/certifaction-local-api-openapi.yml
  type: apiKey
  usage: Server-side integration. API keys are managed from the Certifaction web application.
- in: header
  name: access_token
  parameter: Authorization
  scheme: bearer
  sources:
  - https://developers.certifaction.com/en/references/authentication
  type: oauth2
  usage: Access tokens issued by the customer or by an external OIDC provider that Certifaction has registered. Passed in the Authorization header (CLI `-t/--token`).
slug: certifaction-authentication
source_filename: certifaction-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.certifaction.com/en/references/authentication\ndocs: https://developers.certifaction.com/en/references/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - oidc-external\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  usage: Server-side integration. API keys are managed from the Certifaction web application.\n  sources:\n  - openapi/certifaction-admin-api-openapi.yml\n  - openapi/certifaction-local-api-openapi.yml\n- name: access_token\n  type: oauth2\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  usage: >-\n    Access tokens issued by the customer or by an external OIDC provider that\n    Certifaction has registered. Passed in the Authorization header (CLI `-t/--token`).\n  sources:\n  - https://developers.certifaction.com/en/references/authentication\nnotes: >-\n  The OpenAPI declares only the\
  \ api_key scheme; the documented access-token/OIDC\n  option is added from the authentication reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/authentication/certifaction-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Ai Enterprise Software
- Electronic Signature
- Digital Signature
- Document Signing
- Qualified Electronic Signature
- eIDAS
- Privacy
- Compliance
- Identity Verification
- Switzerland
---
