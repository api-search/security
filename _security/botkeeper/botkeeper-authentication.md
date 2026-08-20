---
api_key_in: []
auth_types: []
description: 'Botkeeper publishes no developer authentication documentation. This profile is assembled entirely from probed evidence: the OpenID Connect discovery document for Botkeeper''s production Amazon Cognito user pool, the published runtime configuration of the Botkeeper Partner Portal SPA at https://www.firm.ai/, the API Gateway challenge returned by ipa.botkeeper.com, and the Apollo GraphQL challenge returned by api.firm.ai/graphql. Nothing here is inferred beyond what those responses state.'
kind: authentication
layout: security
method: probed
name: Botkeeper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botkeeper declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Botkeeper
provider_slug: botkeeper
scheme_count: 0
schemes: []
slug: botkeeper-authentication
source_filename: botkeeper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/openid-configuration\nname: Botkeeper authentication profile\ndescription: >-\n  Botkeeper publishes no developer authentication documentation. This profile is\n  assembled entirely from probed evidence: the OpenID Connect discovery document\n  for Botkeeper's production Amazon Cognito user pool, the published runtime\n  configuration of the Botkeeper Partner Portal SPA at https://www.firm.ai/, the\n  API Gateway challenge returned by ipa.botkeeper.com, and the Apollo GraphQL\n  challenge returned by api.firm.ai/graphql. Nothing here is inferred beyond what\n  those responses state.\n\nsecurity_schemes:\n  - name: cognito_oidc\n    type: openIdConnect\n    openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/openid-configuration\n    provider: Amazon Cognito user pool (us-east-1)\n    issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX\n\
  \    custom_domain: https://login.auth.firm.ai\n    endpoints:\n      authorization: https://login.auth.firm.ai/oauth2/authorize\n      token: https://login.auth.firm.ai/oauth2/token\n      userinfo: https://login.auth.firm.ai/oauth2/userInfo\n      revocation: https://login.auth.firm.ai/oauth2/revoke\n      end_session: https://login.auth.firm.ai/logout\n      jwks: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/jwks.json\n    response_types_supported: [code, token]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    scopes_supported: [openid, email, phone, profile]\n    hosted_ui: https://botkeeper-prod.auth.us-east-1.amazoncognito.com\n    applies_to: Botkeeper Partner Portal (www.firm.ai / app.firm.ai)\n  - name: api_gateway_bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    host: ipa.botkeeper.com\n    evidence:\
  \ >-\n      Every path on ipa.botkeeper.com returns HTTP 403\n      {\"message\":\"Missing Authentication Token\"} — the AWS API Gateway signature\n      for an unauthenticated request against an authorizer-protected API. The\n      Partner Portal SPA authenticates against the Cognito pool above and calls\n      this host, so the presented credential is a Cognito-issued JWT.\n    confidence: high\n    inferred: true\n  - name: graphql_session\n    type: session\n    host: api.firm.ai\n    endpoint: https://api.firm.ai/graphql\n    evidence: >-\n      POST returns {\"errors\":[{\"message\":\"Must be logged in\",\"extensions\":\n      {\"code\":\"UNAUTHENTICATED\"}}]}. Introspection is gated; no SDL captured.\n    confidence: high\n\nend_user_authentication:\n  mfa: >-\n    Two-factor authentication and single sign-on are documented for platform\n    users at\n    https://www.botkeeper.com/en/knowledge/two-factor-authentication-and-single-sign-on-sso\n  sso: true\n  sms_otp: true\n  client_side_rate_limits:\n\
  \    note: >-\n      The Partner Portal SPA config publishes its own SMS throttles — 59 seconds\n      between token requests, 5 attempts per hour. Client-side only; not an API\n      rate-limit contract.\n\ndocumentation:\n  developer_auth_page: null\n  api_key_issuance: not documented publicly\n  note: >-\n    There is no public authentication guide, no API key page, and no developer\n    portal. An integrator cannot learn how to authenticate against the User,\n    Bookkeeping or Tasks APIs from anything Botkeeper publishes.\n\ngaps:\n  - No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource on any Botkeeper host\n  - The OIDC discovery document is only reachable if you already know the Cognito pool id\n  - No documented scopes beyond the four standard OIDC scopes\n  - No documented token lifetimes, refresh policy, or client registration path\n\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n    - url: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/openid-configuration\n\
  \      status: 200\n      content_type: application/json\n    - url: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/jwks.json\n      status: 200\n    - url: https://ipa.botkeeper.com/\n      status: 403\n    - url: https://api.firm.ai/graphql\n      status: 500\n    - url: https://www.botkeeper.com/.well-known/openid-configuration\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botkeeper/refs/heads/main/authentication/botkeeper-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Accounting
- Bookkeeping
- Financial-Services
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Banking Data
- Practice Management
- Small Business
---
