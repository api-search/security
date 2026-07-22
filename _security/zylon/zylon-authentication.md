---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Zylon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zylon secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zylon
provider_slug: zylon
scheme_count: 3
schemes:
- description: 'API token passed as `Authorization: Bearer {API_TOKEN}` on every ZylonGPT and Workspace API request.'
  name: BearerToken
  scheme: bearer
  source: docs
  type: http
- description: POST /api/v1/auth/login exchanges email + password for an account session; POST /api/v1/auth/register creates a credentials account. When LDAP is enabled the server attempts LDAP first then falls back to local credentials.
  name: CredentialsSession
  scheme: session
  source: docs
  type: http
- description: SSO login redirects (Google / Microsoft) and integration OAuth flows for Confluence and SharePoint via the Workspace API OpenID & OAuth endpoints.
  name: OpenIDConnect
  source: docs
  type: openIdConnect
slug: zylon-authentication
source_filename: zylon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zylon.ai/en/developer-manual/build-with-zylon/workspace-api/authentication/auth\ndocs: https://docs.zylon.ai/en/developer-manual/build-with-zylon/workspace-api/authentication/openid\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Zylon is deployed on-premise; there is no single hosted base URL. All calls\n    target the customer's own deployment host ({BASE_URL}). Auth is documented,\n    not derived from a published OpenAPI (none is published publicly).\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    API token passed as `Authorization: Bearer {API_TOKEN}` on every ZylonGPT\n    and Workspace API request.\n  source: docs\n- name: CredentialsSession\n  type: http\n  scheme: session\n  description: >-\n    POST /api/v1/auth/login exchanges email + password for an account session;\n    POST /api/v1/auth/register\
  \ creates a credentials account. When LDAP is\n    enabled the server attempts LDAP first then falls back to local credentials.\n  source: docs\n- name: OpenIDConnect\n  type: openIdConnect\n  description: >-\n    SSO login redirects (Google / Microsoft) and integration OAuth flows for\n    Confluence and SharePoint via the Workspace API OpenID & OAuth endpoints.\n  source: docs\ndirectory_integration:\n- Active Directory / LDAP (enterprise directory integration, added v1.56.0)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zylon/refs/heads/main/authentication/zylon-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
---
