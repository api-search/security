---
api_key_in: []
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-web-forms-api-openapi.yml
  format: yaml
  label: AWeber Web Forms API
  slug: aweber-web-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-web-forms-api-openapi.yml
- filename: aweber-integrations-api-openapi.yml
  format: yaml
  label: AWeber Integrations API
  slug: aweber-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-integrations-api-openapi.yml
- filename: aweber-authentication-api-openapi.yml
  format: yaml
  label: AWeber Authentication API
  slug: aweber-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-authentication-api-openapi.yml
- filename: aweber-beta-api-openapi.yml
  format: yaml
  label: AWeber Beta API
  slug: aweber-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-beta-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Aweber Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AWeber secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AWeber
provider_slug: aweber
scheme_count: 1
schemes:
- description: The following endpoints and scopes are used to authenticate.
  flows:
  - authorizationUrl: https://auth.aweber.com/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://auth.aweber.com/oauth2/token
    revokeUrl: https://auth.aweber.com/oauth2/revoke
    scopes: 9
    tokenUrl: https://auth.aweber.com/oauth2/token
  name: OAuth 2.0
  sources:
  - openapi/_original/aweber-api-openapi.yml
  token_transport: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: aweber-authentication
source_filename: aweber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/aweber-api-openapi.yml\ndocs: https://api.aweber.com/#tag/OAuth-2.0-Overview\ndocs_troubleshooting: https://api.aweber.com/#tag/Troubleshooting\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key: false\n  basic: false\n  mtls: false\n  oidc: false\nnote: >-\n  OAuth 2.0 authorization code is the only supported model for new applications — there is no API\n  key, no basic auth and no service-to-service credential. That makes AWeber unusable for\n  unattended automation without a stored per-customer refresh token, and it is why an MCP server\n  for AWeber would need OAuth rather than a key. Registration is split across two account types:\n  a free DEVELOPER account at labs.aweber.com issues the client_id/client_secret and the OAuth\n  Redirect URL, while the data belongs to a separate AWeber CUSTOMER account that grants access.\nschemes:\n  - name: OAuth 2.0\n    type: oauth2\n    sources:\
  \ [openapi/_original/aweber-api-openapi.yml]\n    description: The following endpoints and scopes are used to authenticate.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.aweber.com/oauth2/authorize\n        tokenUrl: https://auth.aweber.com/oauth2/token\n        refreshUrl: https://auth.aweber.com/oauth2/token\n        revokeUrl: https://auth.aweber.com/oauth2/revoke\n        scopes: 9\n    token_transport: 'Authorization: Bearer <access_token>'\nclient_types:\n  - type: confidential\n    holds_secret: true\n    pkce: forbidden\n    error_if_wrong: 'Confidential Client MUST NOT Use PKCE / code_challenge and code_challenge_method are disallowed for confidential clients'\n  - type: public\n    holds_secret: false\n    pkce: required\n    examples: [mobile applications, WordPress plugins]\n    error_if_wrong: 'Public Client MUST Use PKCE / code_challenge is required for public client'\nregistration:\n  developer_portal: https://labs.aweber.com\n  create_app:\
  \ https://labs.aweber.com/apps\n  login: https://labs.aweber.com/auth/login\n  cost: free\n  note: >-\n    The developer account is unrelated to a customer account. A one-month free customer trial is\n    the documented way to get test data.\nredirect_uri:\n  requirement: >-\n    Must match the OAuth Redirect URL registered for the application EXACTLY. A character\n    difference produces the documented \"Invalid redirect URI\" failure.\nauthorize_url_params: [response_type=code, client_id, redirect_uri, scope, state]\ntokens:\n  refresh_supported: true\n  revocation_supported: true\n  revoke_endpoint: https://auth.aweber.com/oauth2/revoke\n  expiry_documented: >-\n    The token response carries expires_in; a fixed lifetime is not published in the reference.\ndiscovery:\n  rfc8414: false\n  oidc: false\n  note: >-\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration both return 404\n    on auth.aweber.com — endpoints and scopes are discoverable only from the\
  \ documentation. See\n    well-known/aweber-well-known.yml.\nlegacy:\n  oauth1a:\n    status: legacy-still-live\n    endpoints: [POST /oauth/request_token, POST /oauth/access_token]\n    evidence: >-\n      An unauthenticated GET https://api.aweber.com/1.0/accounts returns 400 \"Missing oauth\n      parameters: oauth_consumer_key\" (probed 2026-08-13), and the OAuth 1.0a reference is still\n      published.\n    guidance: AWeber requires OAuth 2.0 for all new applications.\nscopes_detail: scopes/aweber-scopes.yml\nerrors:\n  - {message: Invalid Token, status: 401, cause: Token expired, revoked by the customer, or mistyped}\n  - {message: Invalid Account, status: 401, cause: The AWeber customer account is no longer active}\n  - {message: Invalid Request, status: 401, cause: The request did not use OAuth 2.0}\n  - {message: Consumer key is invalid., status: 401, cause: Bad client credentials}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/authentication/aweber-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
- Web Forms
- Segments
- Webhooks
- OAuth 2.0
- Small Business
---
