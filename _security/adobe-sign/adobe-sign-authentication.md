---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Adobe Acrobat Sign REST API
  slug: adobe-acrobat-sign-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/acrobat-sign/docs/overview/sdks/openapi
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Sign Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Adobe Acrobat Sign secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Adobe Acrobat Sign
provider_slug: adobe-sign
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code flow. The authorization code is exchanged at POST /oauth/v2/token for an access token (~3600s) and a refresh token. Scope modifiers :self, :group, and :account determine the authorization level.
  flows:
  - authorizationUrl: https://secure.adobesign.com/public/oauth/v2
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://secure.adobesign.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/adobe-sign-openapi.yml
  type: oauth2
slug: adobe-sign-authentication
source_filename: adobe-sign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-sign-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.adobesign.com/public/oauth/v2\n    tokenUrl: https://secure.adobesign.com/oauth/v2/token\n    scopes: 12\n  description: OAuth 2.0 authorization-code flow. The authorization code is exchanged at POST\n    /oauth/v2/token for an access token (~3600s) and a refresh token. Scope modifiers :self,\n    :group, and :account determine the authorization level.\n  sources:\n  - openapi/adobe-sign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-sign/refs/heads/main/authentication/adobe-sign-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Electronic Signature
- E-Signature
- Document Workflow
- Digital Signature
- Adobe
- Agreements
---
