---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Omni Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Omni Analytics secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Omni Analytics
provider_slug: omni-analytics
scheme_count: 2
schemes:
- description: Omni API key sent as a bearer token in the Authorization header.
  location: header
  name: bearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.1 browser flow (Personal Access Tokens); Omni provisions API keys on your behalf.
  flow: authorizationCode
  name: oauth2
  type: oauth2
  version: '2.1'
slug: omni-analytics-authentication
source_filename: omni-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.omni.co/docs/API\ndocs: https://docs.omni.co/docs/API\nsummary:\n  types:\n  - http\n  - oauth2\n  http_scheme: bearer\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    The Omni REST API accepts HTTPS only. Requests authenticate with an API key\n    presented as a bearer token in the Authorization header. OAuth 2.1 is also\n    supported (recommended for the MCP server and CLI): a browser flow under\n    which Omni creates API keys automatically; requires Personal Access Tokens\n    to be enabled. API keys are managed under the account's API tokens settings.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  location: header\n  description: Omni API key sent as a bearer token in the Authorization header.\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  version: '2.1'\n  description: OAuth 2.1 browser flow (Personal Access Tokens); Omni provisions API keys on your behalf.\nidentity_providers:\n\
  \  note: >-\n    For instance sign-in Omni supports SAML/OIDC IdPs (Microsoft Entra, Okta,\n    Google Workspace) and SCIM auto-provisioning; these govern user login, not\n    the REST API bearer/OAuth described above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omni-analytics/refs/heads/main/authentication/omni-analytics-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Analytics
- Business Intelligence
- Embedded Analytics
- Semantic Layer
- Artificial Intelligence
- Data
- MCP
---
