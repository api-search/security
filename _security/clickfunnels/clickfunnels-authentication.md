---
api_key_in: []
api_specs:
- filename: clickfunnels-api-openapi.json
  format: json
  label: ClickFunnels API
  slug: clickfunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Clickfunnels Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ClickFunnels secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ClickFunnels
provider_slug: clickfunnels
scheme_count: 2
schemes:
- description: ClickFunnels 2.0 API access token. Team-scoped by default — a default token reaches every workspace in the team that issued it.
  issued_from: Team settings → the CF2 developer portal in the ClickFunnels UI.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clickfunnels-api-openapi.json
  - https://developers.myclickfunnels.com/docs/authentication
  type: http
- artifact: scopes/clickfunnels-scopes.yml
  description: Platform application flow — a third party gets a workspace-scoped access token to act on a ClickFunnels customer's behalf. Not present in the OpenAPI securitySchemes; documented in the OAuth guide and in RFC 8414 metadata.
  flows:
  - authorizationUrl: https://accounts.myclickfunnels.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://accounts.myclickfunnels.com/oauth/register
    revocationUrl: https://accounts.myclickfunnels.com/oauth/revoke
    scopes:
    - admin
    - read
    - write
    - delete
    - mcp
    tokenUrl: https://accounts.myclickfunnels.com/oauth/token
  name: OAuth2
  sources:
  - https://developers.myclickfunnels.com/docs/oauth-20
  - https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server
  type: oauth2
slug: clickfunnels-authentication
source_filename: clickfunnels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.myclickfunnels.com/docs/authentication\ndocs:\n- https://developers.myclickfunnels.com/docs/authentication\n- https://developers.myclickfunnels.com/docs/oauth-20\n- https://developers.myclickfunnels.com/docs/getting-started\n- https://developers.myclickfunnels.com/docs/sso\n- https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  mtls: false\n  openid_connect: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: ClickFunnels 2.0 API access token. Team-scoped by default — a default token reaches every workspace\n    in the team that issued it.\n  sources:\n  - openapi/clickfunnels-api-openapi.json\n  - https://developers.myclickfunnels.com/docs/authentication\n  issued_from: Team settings → the CF2 developer portal in the ClickFunnels\
  \ UI.\n- name: OAuth2\n  type: oauth2\n  description: Platform application flow — a third party gets a workspace-scoped access token to act on a ClickFunnels\n    customer's behalf. Not present in the OpenAPI securitySchemes; documented in the OAuth guide and in RFC\n    8414 metadata.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.myclickfunnels.com/oauth/authorize\n    tokenUrl: https://accounts.myclickfunnels.com/oauth/token\n    revocationUrl: https://accounts.myclickfunnels.com/oauth/revoke\n    registrationUrl: https://accounts.myclickfunnels.com/oauth/register\n    pkce:\n    - S256\n    scopes:\n    - admin\n    - read\n    - write\n    - delete\n    - mcp\n  sources:\n  - https://developers.myclickfunnels.com/docs/oauth-20\n  - https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server\n  artifact: scopes/clickfunnels-scopes.yml\nrequired_headers:\n- header: Authorization\n  value: Bearer <token>\n- header: User-Agent\n  value: YourAppYourOrg\n\
  \  note: Required — ClickFunnels rejects requests without a User-Agent.\nhost_routing:\n  account_level: https://accounts.myclickfunnels.com/api/v2\n  workspace_level: https://{subdomain}.myclickfunnels.com/api/v2\n  note: After an OAuth exchange, prefix workspace-scoped calls with the workspace_url returned in the token\n    response rather than assuming a host.\ntoken_lifetime:\n  expires: false\n  refresh: refresh_token grant advertised in metadata; the OAuth guide says tokens do not expire and expires_in\n    should be ignored.\nother_flows:\n- name: SSO (JWT)\n  description: Authenticate a ClickFunnels contact from your own platform with a signed JWT.\n  docs: https://developers.myclickfunnels.com/docs/sso\n- name: CLI browser login\n  description: cf auth login runs a browser authorization; cf auth login --installation issues a persistent\n    workspace-scoped installation token for service accounts.\n  docs: https://github.com/clickfunnels/cli\nplan_gate: Full API and webhook access\
  \ is not included on the Launch plan.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/authentication/clickfunnels-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Sales Funnels
- Landing Pages
- E-commerce
- Marketing
- Checkout
- CRM
- Email Marketing
- Online Courses
- Webhooks
- Website Builder
- Subscriptions
- Marketing Automation
- Agent Skills
---
