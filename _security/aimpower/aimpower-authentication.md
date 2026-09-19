---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'How callers authenticate to Brainsuite. There is no public OpenAPI, so this profile is built from documents the provider actually serves anonymously rather than derived from a spec. Platform sign-in is OpenID Connect against an Amazon Cognito user pool the company operates in eu-central-1, fronted by its own authorization-server domain auth.brainsuite.ai. The Creative Effectiveness API is a separate, entirely closed surface: every path on api.brainsuite.ai answers HTTP 401 {"message":"Unauthorized"} to an anonymous caller, and the provider states that API credentials are issued on request.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Aimpower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brainsuite.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Brainsuite.ai
provider_slug: aimpower
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.brainsuite.ai/oauth2/authorize
  bearer_format: JWT
  end_session_endpoint: https://auth.brainsuite.ai/logout
  id: oidc-cognito
  id_token_signing_alg_values_supported:
  - RS256
  in: header
  issuer: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB
  jwks_uri: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/jwks.json
  name: Brainsuite platform sign-in (OpenID Connect / Amazon Cognito)
  note: The user-pool web client id is published in the company's own anonymous frontend configuration document, as is normal for a public OAuth client. mandatorySignIn is false in that document, which is a client-side flag for the SPA bootstrap, not a statement that API resources are open - they are not.
  openid_configuration: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/openid-configuration
  region: eu-central-1
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://auth.brainsuite.ai/oauth2/revoke
  scheme: bearer
  scopes: scopes/aimpower-scopes.yml
  subject_types_supported:
  - public
  token_endpoint: https://auth.brainsuite.ai/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  user_pool: eu-central-1_i8L26ssHB
  userinfo_endpoint: https://auth.brainsuite.ai/oauth2/userInfo
  web_client_id_public: true
- evidence:
  - status: 401
    url: https://api.brainsuite.ai/brainsuite
  - status: 401
    url: https://api.brainsuite.ai/openapi.json
  - note: Read through the Zendesk Help Center API; the HTML view answers 403 to crawlers.
    status: 200
    url: https://brainsuite.zendesk.com/hc/en-us/articles/25862139707549-Introducing-the-Brainsuite-API
  id: api-credentials
  name: Creative Effectiveness API credentials
  note: The provider's own support article "Introducing the Brainsuite API" states step one of onboarding is "Request API credentials & documentation". No credential format, header name, key prefix, or token-exchange flow is published anywhere public. Anonymous requests to every probed path on api.brainsuite.ai return HTTP 401 with the body {"message":"Unauthorized"} - the AWS API Gateway default - which reveals that the surface is authorizer-protected but not which scheme it uses.
  status: gated
  type: unknown
slug: aimpower-authentication
source_filename: aimpower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-09-14) plus the anonymous runtime configuration document at\n  https://api.brainsuite.ai/brainsuite/frontend-configuration/v2/configuration (HTTP 200) and\n  the published support article\n  https://brainsuite.zendesk.com/hc/en-us/articles/22152596932253-What-about-privacy-issues-such-as-server-locations\ndescription: >-\n  How callers authenticate to Brainsuite. There is no public OpenAPI, so this profile is\n  built from documents the provider actually serves anonymously rather than derived from a\n  spec. Platform sign-in is OpenID Connect against an Amazon Cognito user pool the company\n  operates in eu-central-1, fronted by its own authorization-server domain\n  auth.brainsuite.ai. The Creative Effectiveness API is a separate, entirely closed surface:\n  every path on api.brainsuite.ai answers\
  \ HTTP 401 {\"message\":\"Unauthorized\"} to an\n  anonymous caller, and the provider states that API credentials are issued on request.\n\napi_host: https://api.brainsuite.ai/brainsuite\npublic_reference_published: false\n\nschemes:\n- id: oidc-cognito\n  type: openIdConnect\n  name: Brainsuite platform sign-in (OpenID Connect / Amazon Cognito)\n  in: header\n  scheme: bearer\n  bearer_format: JWT\n  openid_configuration: >-\n    https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/openid-configuration\n  issuer: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB\n  jwks_uri: >-\n    https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/jwks.json\n  authorization_endpoint: https://auth.brainsuite.ai/oauth2/authorize\n  token_endpoint: https://auth.brainsuite.ai/oauth2/token\n  userinfo_endpoint: https://auth.brainsuite.ai/oauth2/userInfo\n  revocation_endpoint: https://auth.brainsuite.ai/oauth2/revoke\n  end_session_endpoint:\
  \ https://auth.brainsuite.ai/logout\n  response_types_supported: [code, token]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  subject_types_supported: [public]\n  scopes: scopes/aimpower-scopes.yml\n  user_pool: eu-central-1_i8L26ssHB\n  region: eu-central-1\n  web_client_id_public: true\n  note: >-\n    The user-pool web client id is published in the company's own anonymous frontend\n    configuration document, as is normal for a public OAuth client. mandatorySignIn is\n    false in that document, which is a client-side flag for the SPA bootstrap, not a\n    statement that API resources are open - they are not.\n\n- id: api-credentials\n  type: unknown\n  name: Creative Effectiveness API credentials\n  status: gated\n  note: >-\n    The provider's own support article \"Introducing the Brainsuite API\" states step one of\n    onboarding is \"Request API credentials & documentation\". No credential\
  \ format, header\n    name, key prefix, or token-exchange flow is published anywhere public. Anonymous\n    requests to every probed path on api.brainsuite.ai return HTTP 401 with the body\n    {\"message\":\"Unauthorized\"} - the AWS API Gateway default - which reveals that the\n    surface is authorizer-protected but not which scheme it uses.\n  evidence:\n  - url: https://api.brainsuite.ai/brainsuite\n    status: 401\n  - url: https://api.brainsuite.ai/openapi.json\n    status: 401\n  - url: https://brainsuite.zendesk.com/hc/en-us/articles/25862139707549-Introducing-the-Brainsuite-API\n    status: 200\n    note: Read through the Zendesk Help Center API; the HTML view answers 403 to crawlers.\n\nenterprise_sso:\n  supported: true\n  detail: >-\n    \"Optionally, login via corporate single sign on identity management can be integrated.\"\n    SSO is also listed as an entitlement from the Advanced plan upward on the pricing page.\n  docs: https://brainsuite.zendesk.com/hc/en-us/articles/22152596932253-What-about-privacy-issues-such-as-server-locations\n\
  \ntransport:\n  tls_required: true\n  detail: Data transfer via HTTPS; server-side encryption with Amazon SSE-S3 at rest.\n\ngaps:\n- No public API reference, so the API's own authentication scheme is unverifiable from outside.\n- No /.well-known/oauth-protected-resource on the API host (401), so an agent cannot\n  discover the authorization server from the resource server.\n- No security.txt on any company-controlled host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimpower/refs/heads/main/authentication/aimpower-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative Effectiveness
- Ad Testing
- Market Research
- Consumer Neuroscience
- Media
- Software-as-a-Service
- Germany
---
