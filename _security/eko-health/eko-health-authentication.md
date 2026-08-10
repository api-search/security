---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- undocumented
description: ''
kind: authentication
layout: security
method: searched
name: Eko Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Eko Health secures its APIs with oauth2, openIdConnect, and undocumented across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Eko Health
provider_slug: eko-health
scheme_count: 3
schemes:
- applies_to: https://www.ekohealth.com (storefront, customer account, /api/mcp)
  authorization_endpoint: https://account.ekohealth.com/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.ekohealth.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/7156111
  jwks_uri: https://account.ekohealth.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://www.ekohealth.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/eko-health-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://account.ekohealth.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- applies_to: https://www.ekohealth.com
  authorization_servers:
  - https://account.ekohealth.com
  - https://shopify.com/authentication/7156111
  bearer_methods_supported:
  - header
  name: oauth-protected-resource
  sources:
  - well-known/eko-health-oauth-protected-resource.json
  type: oauth2
- applies_to: https://api.ekodevices.com
  name: eko-connect-api
  observed: Unauthenticated GET https://api.ekodevices.com/api/v1/recordings returns HTTP 401 with a 60-byte body, confirming a token/credential-gated REST surface. Neither /oauth/authorize nor /oauth/token exists (404), and no OIDC or RFC 8414 metadata is served on the host, so the credential model is not publicly disclosed. Eko issues Enterprise SDK credentials through sales.
  sources:
  - live probe 2026-08-04
  type: undocumented
slug: eko-health-authentication
source_filename: eko-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://www.ekohealth.com/.well-known/openid-configuration\ndocs: https://support.ekohealth.com/hc/en-us\nnotes: >-\n  Eko Health publishes no OpenAPI, so this profile was NOT derived from securitySchemes.\n  It is assembled from two live, anonymously fetched sources: the OAuth/OIDC discovery\n  documents served on www.ekohealth.com (which govern the storefront + customer-account\n  + MCP surface), and an observed 401 challenge on the Eko Connect API host. Nothing\n  here is inferred beyond those observations.\nsummary:\n  types: [oauth2, openIdConnect, undocumented]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  applies_to: https://www.ekohealth.com (storefront, customer account, /api/mcp)\n  openIdConnectUrl: https://www.ekohealth.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7156111\n\
  \  authorization_endpoint: https://account.ekohealth.com/authentication/oauth/authorize\n  token_endpoint: https://account.ekohealth.com/authentication/oauth/token\n  end_session_endpoint: https://account.ekohealth.com/authentication/logout\n  jwks_uri: https://account.ekohealth.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/eko-health-openid-configuration.json]\n- name: oauth-protected-resource\n  type: oauth2\n  applies_to: https://www.ekohealth.com\n  bearer_methods_supported:\
  \ [header]\n  authorization_servers:\n  - https://account.ekohealth.com\n  - https://shopify.com/authentication/7156111\n  sources: [well-known/eko-health-oauth-protected-resource.json]\n- name: eko-connect-api\n  type: undocumented\n  applies_to: https://api.ekodevices.com\n  observed: >-\n    Unauthenticated GET https://api.ekodevices.com/api/v1/recordings returns HTTP 401\n    with a 60-byte body, confirming a token/credential-gated REST surface. Neither\n    /oauth/authorize nor /oauth/token exists (404), and no OIDC or RFC 8414 metadata is\n    served on the host, so the credential model is not publicly disclosed. Eko issues\n    Enterprise SDK credentials through sales.\n  sources: [live probe 2026-08-04]\nanonymous_surfaces:\n- url: https://www.ekohealth.com/api/mcp\n  note: MCP tools/list succeeds with no credentials (HTTP 200).\n- url: https://www.ekohealth.com/.well-known/ucp\n  note: UCP merchant profile is public.\ngated_surfaces:\n- url: https://www.ekohealth.com/api/ucp/mcp\n\
  \  note: HTTP 422 invalid_profile_url — requires a caller-supplied agent profile URI.\n- url: https://api.ekodevices.com/api/v1/recordings\n  note: HTTP 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eko-health/refs/heads/main/authentication/eko-health-authentication.yml
summary_line: oauth2/openIdConnect/undocumented · 3 schemes
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Digital Health
- Telehealth
- Artificial Intelligence
- Cardiology
- Remote Patient Monitoring
- Commerce
---
