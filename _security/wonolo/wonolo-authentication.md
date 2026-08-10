---
api_key_in:
- body
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wonolo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wonolo secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wonolo
provider_slug: wonolo
scheme_count: 3
schemes:
- description: API V2 callers POST an issued api_key and secret_key to /api_v2/authenticate and receive a token that is presented on subsequent calls. Credentials are issued by Wonolo to customers; there is no public self-service key issuance.
  name: wonolo-api-v2-token
  scheme: bearer
  source: https://wonolo.readme.io/docs/getting-started
  token_endpoint: https://api.wonolo.com/api_v2/authenticate
  type: http
  verified: false
- description: Outbound webhook callbacks are authenticated to the receiver with an X-Wonolo-Webhook-Token header carrying a SHA-256 digest of the webhook JSON body concatenated with the customer's secret API key. The receiving URI must accept HTTPS.
  in: header
  name: wonolo-webhook-signature
  parameter_name: X-Wonolo-Webhook-Token
  source: https://wonolo.readme.io/docs/webhooks
  type: apiKey
  verified: false
- bearer_methods_supported:
  - header
  description: api.wonolo.com is fronted by Pomerium, which publishes OAuth 2.0 authorization-server metadata (RFC 8414) and protected-resource metadata (RFC 9728) at the host root. This is the identity-aware proxy's own OAuth surface — it is not documented by Wonolo as the API V2 application auth model — but it is live, anonymous and machine readable.
  flows:
  - authorizationUrl: https://api.wonolo.com/.pomerium/mcp/authorize
    flow: authorizationCode
    scopes: {}
    tokenUrl: https://api.wonolo.com/.pomerium/mcp/token
  issuer: https://api.wonolo.com
  name: pomerium-oauth2
  pkce:
  - S256
  registration_endpoint: https://api.wonolo.com/.pomerium/mcp/register
  revocation_endpoint: https://api.wonolo.com/.pomerium/mcp/revoke
  source: well-known/wonolo-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  type: oauth2
  verified: true
slug: wonolo-authentication
source_filename: wonolo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://api.wonolo.com/.well-known/oauth-authorization-server\ndocs: https://wonolo.readme.io/docs/getting-started\ndocs_status: 404\nnotes: >-\n  Wonolo publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  assembled from two sources of different strength, kept separate on purpose: (1) the RFC 8414\n  / RFC 9728 metadata documents that api.wonolo.com actually serves anonymously today, fetched\n  verbatim into well-known/; and (2) the API V2 token-exchange model as published on Wonolo's\n  ReadMe developer documentation, which now returns HTTP 404 and could not be re-fetched during\n  this pass. Anything from source (2) is flagged verified: false — do not treat it as confirmed.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [body]\n  oauth2_flows: [authorizationCode]\n  oauth2_scope_count: 0\nschemes:\n- name: wonolo-api-v2-token\n  type: http\n  scheme: bearer\n  verified: false\n  description:\
  \ >-\n    API V2 callers POST an issued api_key and secret_key to /api_v2/authenticate and receive a\n    token that is presented on subsequent calls. Credentials are issued by Wonolo to customers;\n    there is no public self-service key issuance.\n  token_endpoint: https://api.wonolo.com/api_v2/authenticate\n  source: https://wonolo.readme.io/docs/getting-started\n- name: wonolo-webhook-signature\n  type: apiKey\n  in: header\n  parameter_name: X-Wonolo-Webhook-Token\n  verified: false\n  description: >-\n    Outbound webhook callbacks are authenticated to the receiver with an X-Wonolo-Webhook-Token\n    header carrying a SHA-256 digest of the webhook JSON body concatenated with the customer's\n    secret API key. The receiving URI must accept HTTPS.\n  source: https://wonolo.readme.io/docs/webhooks\n- name: pomerium-oauth2\n  type: oauth2\n  verified: true\n  description: >-\n    api.wonolo.com is fronted by Pomerium, which publishes OAuth 2.0 authorization-server\n    metadata (RFC\
  \ 8414) and protected-resource metadata (RFC 9728) at the host root. This is\n    the identity-aware proxy's own OAuth surface — it is not documented by Wonolo as the API V2\n    application auth model — but it is live, anonymous and machine readable.\n  issuer: https://api.wonolo.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.wonolo.com/.pomerium/mcp/authorize\n    tokenUrl: https://api.wonolo.com/.pomerium/mcp/token\n    scopes: {}\n  registration_endpoint: https://api.wonolo.com/.pomerium/mcp/register\n  revocation_endpoint: https://api.wonolo.com/.pomerium/mcp/revoke\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, none]\n  bearer_methods_supported: [header]\n  source: well-known/wonolo-oauth-authorization-server.json\naccess_levels:\n- name: Public Pool\n  verified: false\n  description: >-\n    Access to Wonolo's public pool of workers. Write operations are forbidden in many cases at\n    this level.\n  source: https://wonolo.readme.io/docs/getting-started\n\
  - name: Private Pool\n  verified: false\n  description: For companies managing their own private pool of workers.\n  source: https://wonolo.readme.io/docs/getting-started\nx-evidence:\n- {url: 'https://api.wonolo.com/.well-known/oauth-authorization-server', status: 200, fetched: '2026-08-05'}\n- {url: 'https://api.wonolo.com/.well-known/oauth-protected-resource', status: 200, fetched: '2026-08-05'}\n- {url: 'https://api.wonolo.com/api_v2/info', status: 200, fetched: '2026-08-05'}\n- {url: 'https://wonolo.readme.io/docs/getting-started', status: 404, fetched: '2026-08-05'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonolo/refs/heads/main/authentication/wonolo-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Staffing
- Workforce
- Human Resources
- Marketplace
- Gig Economy
- Recruiting
- Labor
- On-Demand
---
