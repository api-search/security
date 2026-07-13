---
api_key_in:
- header
api_specs:
- filename: docusign-openapi-original.yml
  format: yaml
  label: Docusign eSignature REST API
  slug: docusign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-openapi-original.yml
- filename: docusign-admin-openapi-original.yml
  format: yaml
  label: Docusign Admin API
  slug: docusign-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-admin-openapi-original.yml
- filename: docusign-click-openapi-original.yml
  format: yaml
  label: Docusign Click API
  slug: docusign-click-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-click-openapi-original.yml
- filename: docusign-maestro-openapi-original.yml
  format: yaml
  label: Docusign Maestro API
  slug: docusign-maestro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-maestro-openapi-original.yml
- filename: docusign-monitor-openapi-original.yml
  format: yaml
  label: Docusign Monitor API
  slug: docusign-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-monitor-openapi-original.yml
- filename: docusign-rooms-openapi-original.yml
  format: yaml
  label: Docusign Rooms API
  slug: docusign-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-rooms-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Docusign Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Docusign secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Docusign
provider_slug: docusign
scheme_count: 3
schemes:
- description: OAuth2 Access code Grant
  flows:
  - authorizationUrl: https://account.docusign.com/oauth/auth
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://account.docusign.com/oauth/auth
  name: accessCode
  sources:
  - openapi/docusign-admin-openapi-original.yml
  - openapi/docusign-maestro-openapi-original.yml
  type: oauth2
- description: DocuSign uses OAuth 2.0. Supports Authorization Code Grant for user-present applications and JWT Grant for service integrations.
  flows:
  - authorizationUrl: https://account-d.docusign.com/oauth/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://account-d.docusign.com/oauth/token
  - authorizationUrl: https://account-d.docusign.com/oauth/auth
    flow: implicit
    scopes: 1
  name: OAuth2
  sources:
  - openapi/docusign-esignature-openapi.yml
  type: oauth2
- in: header
  name: DSBearerAuth
  parameter: Authorization
  sources:
  - openapi/docusign-maestro-openapi-original.yml
  - openapi/docusign-monitor-openapi-original.yml
  - openapi/docusign-rooms-openapi-original.yml
  type: apiKey
slug: docusign-authentication
source_filename: docusign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docusign-admin-openapi-original.yml, openapi/docusign-esignature-openapi.yml,\n  openapi/docusign-maestro-openapi-original.yml, openapi/docusign-monitor-openapi-original.yml,\n  openapi/docusign-rooms-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: accessCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.docusign.com/oauth/auth\n    tokenUrl: https://account.docusign.com/oauth/auth\n    scopes: 9\n  description: OAuth2 Access code Grant\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n  - openapi/docusign-maestro-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account-d.docusign.com/oauth/auth\n    tokenUrl: https://account-d.docusign.com/oauth/token\n    scopes: 3\n \
  \ - flow: implicit\n    authorizationUrl: https://account-d.docusign.com/oauth/auth\n    scopes: 1\n  description: DocuSign uses OAuth 2.0. Supports Authorization Code Grant for user-present applications\n    and JWT Grant for service integrations.\n  sources:\n  - openapi/docusign-esignature-openapi.yml\n- name: DSBearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/docusign-maestro-openapi-original.yml\n  - openapi/docusign-monitor-openapi-original.yml\n  - openapi/docusign-rooms-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/authentication/docusign-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
---
