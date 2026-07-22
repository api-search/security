---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Matik Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Matik secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Matik
provider_slug: matik
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.matik.io/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.matik.io/api/v1/oauth/token/
    scopes:
      consumer: End-user access — generate presentations/documents from existing templates.
      producer: Administrative access — create/manage templates, data sources, and content.
    tokenUrl: https://app.matik.io/api/v1/oauth/token/
  name: OAuth2
  sources:
  - https://developer.matik.io/guides/oauth
  type: oauth2
slug: matik-authentication
source_filename: matik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.matik.io/guides/oauth\ndocs: https://developer.matik.io/guides/oauth\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  api_key_in: []\n  bearer: true\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.matik.io/oauth/authorize\n        tokenUrl: https://app.matik.io/api/v1/oauth/token/\n        refreshUrl: https://app.matik.io/api/v1/oauth/token/\n        scopes:\n          producer: Administrative access — create/manage templates, data sources, and content.\n          consumer: End-user access — generate presentations/documents from existing templates.\n    sources: [https://developer.matik.io/guides/oauth]\nrequest:\n  header: 'Authorization: Bearer {access_token}'\n  content_type: application/json\nnotes: >-\n  Register client credentials (client id + secret) with producer and consumer scopes.\n\
  \  Access tokens are bearer tokens presented against the REST API base https://app.matik.io/api/1.0/.\n  The MCP server uses the same OAuth 2.0 model with dynamic client registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matik/refs/heads/main/authentication/matik-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Content Automation
- Presentations
- Documents
- Data-Driven Content
- Sales Enablement
- Customer Success
- Revenue Operations
- AI
- MCP
---
