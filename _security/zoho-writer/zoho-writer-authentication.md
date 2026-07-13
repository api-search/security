---
api_key_in: []
api_specs:
- filename: zoho-writer-openapi.json
  format: json
  label: Zoho Writer API
  slug: zoho-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-writer/refs/heads/main/openapi/zoho-writer-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Writer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Writer secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Writer
provider_slug: zoho-writer
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Refer to https://www.zoho.com/writer/help/api/v1/oauth-2.html for setup.
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: OAuth2
  sources:
  - openapi/zoho-writer-openapi.json
  type: oauth2
slug: zoho-writer-authentication
source_filename: zoho-writer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoho-writer-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 6\n  description: OAuth 2.0 authentication. Refer to https://www.zoho.com/writer/help/api/v1/oauth-2.html\n    for setup.\n  sources:\n  - openapi/zoho-writer-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-writer/refs/heads/main/authentication/zoho-writer-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Documents
- Word Processor
- Mail Merge
- Document Generation
- Electronic Signatures
- Zoho
- Office Suite
- Automation
---
