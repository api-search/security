---
api_key_in: []
api_specs:
- filename: frameio-v4-openapi.json
  format: json
  label: Frame.io V4 API
  slug: frameio-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-v4-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Frameio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Frame.io secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Frame.io
provider_slug: frameio
scheme_count: 2
schemes:
- description: 'For more information, see: https://developer.adobe.com/frameio'
  flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: OAuth2
  sources:
  - openapi/frameio-v4-openapi.json
  type: oauth2
- description: Server to server authentication flow
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: s2s_auth
  sources:
  - openapi/frameio-v4-openapi.json
  type: oauth2
slug: frameio-authentication
source_filename: frameio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/frameio-v4-openapi.json\ndocs: https://next.developer.frame.io/platform/v4/docs/guides/authentication/overview\nnote: OAuth2 via Adobe IMS (ims-na1.adobelogin.com). authorizationCode flow for user\n  apps (Web/SPA/Native with PKCE), clientCredentials for server-to-server. Legacy\n  developer tokens supported via the x-frameio-legacy-token-auth header.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 4\n  description: 'For more information, see: https://developer.adobe.com/frameio'\n  sources:\n  - openapi/frameio-v4-openapi.json\n- name: s2s_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n\
  \    scopes: 3\n  description: Server to server authentication flow\n  sources:\n  - openapi/frameio-v4-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/authentication/frameio-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Media
- Video
- Collaboration
- Review and Approval
- Media Production
- Adobe
- Content
---
