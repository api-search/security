---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pega Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Pega secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Pega
provider_slug: pega
scheme_count: 2
schemes:
- flow: clientCredentials
  grant: client_credentials
  name: OAuth2 Client Credentials
  role_binding: Persona on the Client Registration rule
  token_url_pattern: https://<accessTokenURL>/token
  type: oauth2
  used_for: Server-to-server / external-system DX API integration (create case, get case, run action, query data views).
- flow: authorizationCode
  name: OAuth2 Authorization Code (PKCE)
  pkce: true
  type: oauth2
  used_for: Browser/embedded experiences (e.g. the <pega-embed> web-embed component) acting on behalf of an interactive user.
slug: pega-authentication
source_filename: pega-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/pegasystems/pega-launchpad-agent-skills (launchpad-dx-apis/webembed SKILL.md) + docs.pega.com DX API authentication\ndocs: https://docs.pega.com/bundle/platform/page/platform/dx-api/dx-api-overview.html\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  notes: >-\n    Pega DX APIs authenticate with OAuth 2.0. Access is granted via an OAuth 2.0\n    Client Registration rule in the Pega/Launchpad environment; the Persona bound\n    to the client registration determines the access roles and privileges (and\n    therefore which DX API operations the credentials may invoke). Callers are\n    provisioned an Application URL, an Access Token URL, a Client ID and a Client\n    Secret.\nschemes:\n  - name: OAuth2 Client Credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url_pattern: \"https://<accessTokenURL>/token\"\n    grant: client_credentials\n    used_for:\
  \ Server-to-server / external-system DX API integration (create case, get case, run action, query data views).\n    role_binding: Persona on the Client Registration rule\n  - name: OAuth2 Authorization Code (PKCE)\n    type: oauth2\n    flow: authorizationCode\n    pkce: true\n    used_for: Browser/embedded experiences (e.g. the <pega-embed> web-embed component) acting on behalf of an interactive user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pega/refs/heads/main/authentication/pega-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Low-Code
- Business Process Management
- Workflow Automation
- CRM
- Decisioning
- Artificial Intelligence
- Enterprise
- Case Management
---
