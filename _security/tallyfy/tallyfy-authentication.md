---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tallyfy Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Tallyfy secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Tallyfy
provider_slug: tallyfy
scheme_count: 3
schemes:
- description: 'User (personal) access token tied to a specific user and their exact permissions, obtained from the user profile. Sent as Authorization: Bearer. Invalidated when the user logs out of the Tallyfy web app - not recommended for long-running automations.'
  name: personalAccessToken
  scheme: bearer
  type: http
- description: Application-level credentials (client ID and secret) that let an application act on behalf of multiple users. Ideal for server-to-server connections and long-running automations.
  name: applicationToken
  scheme: bearer
  type: http
- authorizationUrl: https://account.tallyfy.com/oauth/authorize
  description: OAuth 2.0 implicit grant for third-party applications. Users authenticate on Tallyfy's domain; the access token is returned in the redirect URL fragment (token_type=Bearer, expires_in). Available to paid organizations; Client ID is issued by Tallyfy Support. No granular scope surface is documented - the token acts with the authenticating user's permissions.
  flow: implicit
  name: oauth2
  response_type: token
  token_delivery: url-fragment
  type: oauth2
slug: tallyfy-authentication
source_filename: tallyfy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://raw.githubusercontent.com/tallyfy/cli/HEAD/pkg/tallyfy/client.go\ndocs: https://tallyfy.com/products/pro/integrations/open-api/\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  transport_header: 'Authorization: Bearer {access_token}'\n  oauth2_flows: [implicit]\nschemes:\n  - name: personalAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      User (personal) access token tied to a specific user and their exact\n      permissions, obtained from the user profile. Sent as Authorization: Bearer.\n      Invalidated when the user logs out of the Tallyfy web app - not recommended\n      for long-running automations.\n  - name: applicationToken\n    type: http\n    scheme: bearer\n    description: >-\n      Application-level credentials (client ID and secret) that let an application\n      act on behalf of multiple users. Ideal for server-to-server connections and\n      long-running automations.\n\
  \  - name: oauth2\n    type: oauth2\n    flow: implicit\n    authorizationUrl: https://account.tallyfy.com/oauth/authorize\n    response_type: token\n    token_delivery: url-fragment   # access_token returned in the redirect URL fragment\n    description: >-\n      OAuth 2.0 implicit grant for third-party applications. Users authenticate on\n      Tallyfy's domain; the access token is returned in the redirect URL fragment\n      (token_type=Bearer, expires_in). Available to paid organizations; Client ID\n      is issued by Tallyfy Support. No granular scope surface is documented - the\n      token acts with the authenticating user's permissions.\nnotes:\n  - Most endpoints are organization-scoped (/organizations/{org_id}/...); a token is tied to the user's current organization.\n  - No public OpenAPI/Swagger document is served unauthenticated (api.tallyfy.com/openapi.json returns 401); auth model captured from first-party CLI source and docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tallyfy/refs/heads/main/authentication/tallyfy-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Workflow Automation
- Business Process Management
- SOPs
- Tasks
- Approvals
- Forms
- Process Management
- No-Code
---
