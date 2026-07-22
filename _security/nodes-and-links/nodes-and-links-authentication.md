---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nodes And Links Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nodes and Links secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nodes and Links
provider_slug: nodes-and-links
scheme_count: 1
schemes:
- flows:
  - evidence: developer-portal main.js references oauth/token, client_id, scope
    flow: clientCredentials
    tokenUrl: https://api.app.nodeslinks.com/oauth/token
  name: OAuth2
  sources:
  - https://developer.nodeslinks.com/
  type: oauth2
slug: nodes-and-links-authentication
source_filename: nodes-and-links-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.nodeslinks.com/\ndocs: https://developer.nodeslinks.com/\nnotes: >-\n  Nodes & Links exposes a production API at https://api.app.nodeslinks.com behind\n  AWS API Gateway (unauthenticated requests return HTTP 403\n  {\"message\":\"Missing Authentication Token\"}). The developer-portal single-page app\n  (developer.nodeslinks.com) drives an OAuth token exchange against an oauth/token\n  endpoint using client_id + scope, indicating an OAuth 2.0 bearer-token model for\n  programmatic access. No public OpenAPI is published (the reference is served inside\n  the authenticated portal), so security schemes could not be derived mechanically.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.app.nodeslinks.com/oauth/token\n    evidence: developer-portal main.js references\
  \ oauth/token, client_id, scope\n  sources:\n  - https://developer.nodeslinks.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nodes-and-links/refs/heads/main/authentication/nodes-and-links-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Project Management
- Project Controls
- Construction
- Scheduling
- Artificial Intelligence
- Risk Analysis
- Earned Value Management
---
