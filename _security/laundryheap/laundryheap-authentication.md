---
api_key_in: []
auth_types: []
description: Laundryheap runs a full OAuth 2.0 authorization server with OpenID Connect on its own root host. Nothing about it is documented on the public website — it was found only by probing /.well-known/ — but every endpoint it advertises is live and answers with standards-compliant errors, and it advertises a domain-specific `orders.create` scope. This is the company's real authentication surface.
kind: authentication
layout: security
method: probed
name: Laundryheap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laundryheap declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Laundryheap
provider_slug: laundryheap
scheme_count: 2
schemes:
- description: OAuth 2.0 / OpenID Connect provider (Doorkeeper + doorkeeper-openid_connect shape). Supports authorization_code with PKCE for user-delegated access and client_credentials for server-to-server partner access.
  flows:
    authorization_code:
      authorization_url: https://www.laundryheap.com/oauth/authorize
      pkce:
        code_challenge_methods:
        - plain
        - S256
        supported: true
      refresh_url: null
      scopes:
        openid: OpenID Connect — issue an ID token identifying the end user.
        orders.create: Create orders on behalf of the authenticated account. The only business scope the authorization server advertises.
      token_url: https://www.laundryheap.com/oauth/token
    client_credentials:
      scopes:
        orders.create: Create orders as the client itself (server-to-server).
      token_url: https://www.laundryheap.com/oauth/token
  id: oauth2
  issuer: https://www.laundryheap.com
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- description: The first-party web app and the REST/GraphQL surfaces also accept the Rails session cookies (_session_id, _laundry_heap_session) set on any request to www.laundryheap.com. This is the browser path, not an integration path.
  id: session_cookie
  observed: Set-Cookie on GET /api/v1/services (httponly; samesite=lax; secure)
  type: cookie
slug: laundryheap-authentication
source_filename: laundryheap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://www.laundryheap.com/.well-known/openid-configuration (HTTP 200) and\n  live unauthenticated probes of every endpoint it advertises, plus the observed\n  auth behaviour of https://www.laundryheap.com/graphql.\ndescription: >-\n  Laundryheap runs a full OAuth 2.0 authorization server with OpenID Connect on\n  its own root host. Nothing about it is documented on the public website — it\n  was found only by probing /.well-known/ — but every endpoint it advertises is\n  live and answers with standards-compliant errors, and it advertises a\n  domain-specific `orders.create` scope. This is the company's real\n  authentication surface.\n\nprimary_scheme: oauth2\nschemes:\n  - id: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 / OpenID Connect provider (Doorkeeper + doorkeeper-openid_connect\n      shape). Supports authorization_code with PKCE for user-delegated access and\n      client_credentials for server-to-server\
  \ partner access.\n    issuer: https://www.laundryheap.com\n    flows:\n      authorization_code:\n        authorization_url: https://www.laundryheap.com/oauth/authorize\n        token_url: https://www.laundryheap.com/oauth/token\n        refresh_url: null\n        pkce:\n          supported: true\n          code_challenge_methods: [plain, S256]\n        scopes:\n          openid: OpenID Connect — issue an ID token identifying the end user.\n          orders.create: >-\n            Create orders on behalf of the authenticated account. The only\n            business scope the authorization server advertises.\n      client_credentials:\n        token_url: https://www.laundryheap.com/oauth/token\n        scopes:\n          orders.create: Create orders as the client itself (server-to-server).\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    response_types: [code]\n    response_modes: [query, fragment, form_post]\n\n  - id: session_cookie\n    type: cookie\n\
  \    description: >-\n      The first-party web app and the REST/GraphQL surfaces also accept the\n      Rails session cookies (_session_id, _laundry_heap_session) set on any\n      request to www.laundryheap.com. This is the browser path, not an\n      integration path.\n    observed: Set-Cookie on GET /api/v1/services (httponly; samesite=lax; secure)\n\nopenid_connect:\n  discovery: https://www.laundryheap.com/.well-known/openid-configuration\n  document: well-known/laundryheap-openid-configuration.json\n  userinfo_endpoint: https://www.laundryheap.com/oauth/userinfo\n  jwks_uri: https://www.laundryheap.com/oauth/discovery/keys\n  jwks_file: well-known/laundryheap-jwks.json\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims_supported: [iss, sub, aud, exp, iat]\n  claim_types: [normal]\n\ndynamic_client_registration:\n  supported: true\n  spec: RFC 7591\n  endpoint: https://www.laundryheap.com/oauth/registration\n  observed: >-\n    POST with an empty body returns 400\n\
  \    {\"error\":\"invalid_client_params\",\"error_description\":\"Name can't be blank,\n    Redirect URI can't be blank\"} — the endpoint is live and validating, not a\n    stub. GET returns 404.\n  note: >-\n    Open dynamic client registration is unusual for a consumer marketplace and is\n    the strongest single signal that Laundryheap intends third parties to\n    integrate. No published documentation explains who may register.\n\ntoken_management:\n  introspection_endpoint: https://www.laundryheap.com/oauth/introspect\n  introspection_spec: RFC 7662\n  revocation_endpoint: https://www.laundryheap.com/oauth/revoke\n  revocation_spec: RFC 7009\n\ngraphql_authentication:\n  endpoint: https://www.laundryheap.com/graphql\n  anonymous_fields: >-\n    A small number of fields resolve anonymously (__typename, and field-shape\n    errors are returned rather than auth errors for countries/globalSettings).\n    Account fields are gated.\n  gated_response: >-\n    errors[0].message \"Authentication\
  \ needed\" with\n    extensions.short_code \"authentication\" and data.<field> null, returned under\n    HTTP 200 per the GraphQL spec.\n  magic_link: >-\n    The web client also carries an `authorize(email)` mutation and a\n    `signInWithMagicLink(token)` mutation — a passwordless email flow, separate\n    from the OAuth server.\n  social_login: >-\n    Apple (com.LaundryHeap.applelogin), Google (/auth/google) and Facebook\n    (/auth/facebook) sign-in are wired into the web app.\n\nx-evidence:\n  fetched: '2026-08-23'\n  probes:\n    - url: https://www.laundryheap.com/.well-known/openid-configuration\n      status: 200\n    - url: https://www.laundryheap.com/oauth/token\n      method: POST\n      status: 400\n      body: '{\"error\":\"invalid_request\",\"error_description\":\"Missing required parameter: grant_type.\"}'\n    - url: https://www.laundryheap.com/oauth/userinfo\n      status: 401\n    - url: https://www.laundryheap.com/oauth/introspect\n      method: POST\n      status:\
  \ 400\n    - url: https://www.laundryheap.com/oauth/registration\n      method: POST\n      status: 400\n    - url: https://www.laundryheap.com/oauth/revoke\n      method: POST\n      status: 403\n    - url: https://www.laundryheap.com/oauth/discovery/keys\n      status: 200\n\ngaps:\n  - No public developer documentation describes any of this surface.\n  - No published scope reference; `orders.create` is known only from the discovery document.\n  - No documented process for obtaining client credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laundryheap/refs/heads/main/authentication/laundryheap-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Laundry
- Dry Cleaning
- On-Demand Services
- Logistics
- Last Mile Delivery
- Consumer Services
- Hospitality
- Ordering
- GraphQL
- OAuth
---
