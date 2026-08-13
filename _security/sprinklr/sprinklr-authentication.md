---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Sprinklr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwt-bearer
overview: Sprinklr secures its APIs with oauth2, apiKey, and mutualTLS across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and jwt-bearer flow(s).
provider_name: Sprinklr
provider_slug: sprinklr
scheme_count: 5
schemes:
- description: The API key (client_id) issued per environment. Acts as both a unique identifier and a secret token. Sent on every request alongside the bearer token; omitting it yields 403 "Developer Inactive".
  expiry: none
  in: header
  issuance:
    current: All Settings > APIs and Integrations > Developer Tools inside the Sprinklr platform (26.1 release onward).
    docs: https://www.sprinklr.com/help/articles/developer-tools/developer-tools-in-sprinklr/692e8b39f0afa271
    legacy: dev.sprinklr.com developer portal > Apps > + New App
    note: The secret is masked and is revealed only after confirming from an email sent to the registered developer-portal address.
  name: apiKey
  parameter_name: key
  rotation: Keys and secrets do not expire. They are static and can only be deleted or disabled from the customer's Sprinklr developer account.
  type: apiKey
- description: OAuth 2.0 access token, obtained through one of the flows below.
  format: Bearer {access_token}
  in: header
  name: bearerAuth
  parameter_name: Authorization
  scheme: bearer
  type: http
- flows:
  - authorizationUrl: https://api3.sprinklr.com/{env}/oauth/authorize
    code_ttl_note: The authorization code is valid for 10 minutes.
    code_ttl_seconds: 600
    flow: authorizationCode
    label: OAuth 2.0 for Customers (Code Grant)
    refreshUrl: https://api3.sprinklr.com/{env}/oauth/token
    request_content_type: application/x-www-form-urlencoded
    scopes: {}
    scopes_note: Sprinklr's authorize URL takes client_id, response_type and redirect_uri only. No `scope` parameter is documented and no scope registry is published, so scopes/ is deliberately absent from this repo rather than fabricated. Authorization is governed instead by the Sprinklr platform role/permission model and by the partner+client workspace combination the user selects at consent time.
    tokenUrl: https://api3.sprinklr.com/{env}/oauth/token
  - description: Generates a token without an authorization code. Requires a default user to be configured on the Sprinklr side; the token then acts as that user.
    flow: clientCredentials
    label: Client Credentials Grant Type (Default User)
    tokenUrl: https://api3.sprinklr.com/{env}/oauth/token
  - description: Certificate-based JWT token generation, documented alongside the OAuth flows.
    flow: jwt-bearer
    label: JWT Certificate Based Token Generation
  - description: Partner-side SSO variant of the code grant.
    flow: authorizationCode
    label: OAuth 2.0 SSO for Partners
  name: oauth2
  type: oauth2
- description: Mutual TLS Authentication is listed as a supported authorization method in the developer portal's Authorize section. No certificate-issuance procedure is published publicly.
  name: mutualTLS
  type: mutualTLS
- description: The Community APIs use a separate authorization process entirely, requiring a projectId and preSharedKey to mint unauthenticated and authenticated tokens. Sprinklr routes access through a success manager; the endpoints are Create Unauthenticated Token and Create Authenticated Token.
  docs: https://dev.sprinklr.com/community-apis
  in: header
  name: communityToken
  type: apiKey
slug: sprinklr-authentication
source_filename: sprinklr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://dev.sprinklr.com/authorize\ndocs:\n  - https://dev.sprinklr.com/authorize\n  - https://dev.sprinklr.com/api-key-and-secret-generation\n  - https://dev.sprinklr.com/getting-started\n  - https://dev.sprinklr.com/refreshing-access-token\n  - https://dev.sprinklr.com/authorization-troubleshooting\nnote: >-\n  Derived-from-spec is not possible: Sprinklr publishes no OpenAPI, so this\n  profile is read directly from the developer-portal authorization pages.\n  Sprinklr's model is unusual in that BOTH an OAuth 2.0 bearer token AND a\n  static API key are required on every call — the key travels in a bare `key`\n  header, not Authorization.\nsummary:\n  types: [oauth2, apiKey, mutualTLS]\n  api_key_in: [header]\n  api_key_name: key\n  oauth2_flows: [authorizationCode, clientCredentials, jwt-bearer]\n  both_required: true\n  scopes_published: false\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name:\
  \ key\n    description: >-\n      The API key (client_id) issued per environment. Acts as both a unique\n      identifier and a secret token. Sent on every request alongside the bearer\n      token; omitting it yields 403 \"Developer Inactive\".\n    expiry: none\n    rotation: >-\n      Keys and secrets do not expire. They are static and can only be deleted or\n      disabled from the customer's Sprinklr developer account.\n    issuance:\n      current: >-\n        All Settings > APIs and Integrations > Developer Tools inside the\n        Sprinklr platform (26.1 release onward).\n      legacy: dev.sprinklr.com developer portal > Apps > + New App\n      docs: https://www.sprinklr.com/help/articles/developer-tools/developer-tools-in-sprinklr/692e8b39f0afa271\n      note: >-\n        The secret is masked and is revealed only after confirming from an email\n        sent to the registered developer-portal address.\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n\
  \    parameter_name: Authorization\n    format: 'Bearer {access_token}'\n    description: OAuth 2.0 access token, obtained through one of the flows below.\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        label: OAuth 2.0 for Customers (Code Grant)\n        authorizationUrl: 'https://api3.sprinklr.com/{env}/oauth/authorize'\n        tokenUrl: 'https://api3.sprinklr.com/{env}/oauth/token'\n        refreshUrl: 'https://api3.sprinklr.com/{env}/oauth/token'\n        scopes: {}\n        scopes_note: >-\n          Sprinklr's authorize URL takes client_id, response_type and\n          redirect_uri only. No `scope` parameter is documented and no scope\n          registry is published, so scopes/ is deliberately absent from this\n          repo rather than fabricated. Authorization is governed instead by the\n          Sprinklr platform role/permission model and by the partner+client\n          workspace combination the user selects at consent time.\n   \
  \     request_content_type: application/x-www-form-urlencoded\n        code_ttl_seconds: 600\n        code_ttl_note: The authorization code is valid for 10 minutes.\n      - flow: clientCredentials\n        label: Client Credentials Grant Type (Default User)\n        tokenUrl: 'https://api3.sprinklr.com/{env}/oauth/token'\n        description: >-\n          Generates a token without an authorization code. Requires a default\n          user to be configured on the Sprinklr side; the token then acts as\n          that user.\n      - flow: jwt-bearer\n        label: JWT Certificate Based Token Generation\n        description: Certificate-based JWT token generation, documented alongside the OAuth flows.\n      - flow: authorizationCode\n        label: OAuth 2.0 SSO for Partners\n        description: Partner-side SSO variant of the code grant.\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      Mutual TLS Authentication is listed as a supported authorization method in\n  \
  \    the developer portal's Authorize section. No certificate-issuance\n      procedure is published publicly.\n  - name: communityToken\n    type: apiKey\n    in: header\n    description: >-\n      The Community APIs use a separate authorization process entirely,\n      requiring a projectId and preSharedKey to mint unauthenticated and\n      authenticated tokens. Sprinklr routes access through a success manager;\n      the endpoints are Create Unauthenticated Token and Create Authenticated\n      Token.\n    docs: https://dev.sprinklr.com/community-apis\ntoken:\n  type: Bearer\n  access_token_ttl_seconds: 2591999\n  access_token_ttl_human: 30 days\n  refresh:\n    supported: true\n    grant_type: refresh_token\n    single_use: true\n    note: >-\n      The refresh token has no expiry but can be used only once — regenerating\n      produces a new refresh token and invalidates the previous one. Refresh\n      token must be URL-encoded.\n  constraints:\n    - >-\n      ONE TOKEN PER API\
  \ KEY. If two stateless instances share a client_id, the\n      second token generation invalidates the first instance's access AND\n      refresh token. Each instance needs its own key/token pair.\n    - >-\n      Tokens are environment-specific. A key/token minted for one Sprinklr\n      environment returns HTTP 421 Misdirected Request against another.\n    - Tokens remain valid only while the authenticating user's Sprinklr password is valid.\n    - The user must hold the \"Generate Token\" permission inside the Sprinklr platform.\nenvironments:\n  pattern: 'https://api3.sprinklr.com/{env}/api/{version}/{endpoint}'\n  note: >-\n    {env} is the Sprinklr hosting environment (prod0, prod2, prod3, prod4,\n    prod8, ...). For the default Production environment (app.sprinklr.com) the\n    {env} segment is omitted entirely:\n    https://api3.sprinklr.com/api/v1/{endpoint}. Customers find their\n    environment by searching the Sprinklr UI page source for\n    \"sentry-environment\".\nrequired_headers:\n\
  \  - {name: Authorization, value: 'Bearer {access_token}'}\n  - {name: key, value: '{api_key}'}\n  - {name: Content-Type, value: application/json}\ngaps:\n  - No OAuth scopes published; no /.well-known/oauth-authorization-server and no /.well-known/openid-configuration on any Sprinklr host (all 404 — see well-known/).\n  - No public self-service signup that yields a working token; the OAuth flow requires an existing licensed Sprinklr platform account.\n  - Access-token TTL is documented inconsistently (2591999s / 30 days on the getting-started page; 28799s / 8 hours in the refresh-token example response).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprinklr/refs/heads/main/authentication/sprinklr-authentication.yml
summary_line: oauth2/apiKey/mutualTLS · 5 schemes
tags:
- Social Media Management
- Customer Experience
- Customer Service
- Marketing
- Advertising
- Listening
- Publishing
- Reporting
- Unified CXM
---
