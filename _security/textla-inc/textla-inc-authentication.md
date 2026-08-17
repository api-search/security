---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Textla Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Textla Inc. declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Textla Inc.
provider_slug: textla-inc
scheme_count: 0
schemes: []
slug: textla-inc-authentication
source_filename: textla-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.textla.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Textla publishes no developer API and therefore no developer authentication documentation.\n  This profile is derived entirely from the OpenID Connect discovery document Textla serves\n  at auth.textla.com — an Auth0 tenant on a Textla-owned custom domain that fronts sign-in to\n  the app.textla.com application. It describes how HUMANS sign in to the product, not how a\n  third-party developer would authenticate to an API. No API key, personal access token, or\n  developer credential surface is documented anywhere on Textla's public site or help center.\nscope: application-signin\nprovider: Auth0 (custom domain auth.textla.com)\nissuer: https://auth.textla.com/\nsecuritySchemes:\n- name: textla_openid_connect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.textla.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect\
  \ provider fronting the Textla web application. Advertised by Textla's own\n    host; no developer-facing client registration is documented publicly, though the tenant\n    exposes a dynamic registration endpoint.\n  endpoints:\n    authorization: https://auth.textla.com/authorize\n    token: https://auth.textla.com/oauth/token\n    userinfo: https://auth.textla.com/userinfo\n    jwks: https://auth.textla.com/.well-known/jwks.json\n    revocation: https://auth.textla.com/oauth/revoke\n    registration: https://auth.textla.com/oidc/register\n    device_authorization: https://auth.textla.com/oauth/device/code\n    backchannel_authentication: https://auth.textla.com/bc-authorize\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  pkce:\n    supported: true\n    methods:\n    - S256\n\
  \    - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\nobservations:\n- id: pkce-s256\n  value: true\n  evidence: code_challenge_methods_supported includes S256.\n- id: plain-pkce-allowed\n  value: true\n  evidence: >-\n    code_challenge_methods_supported also includes \"plain\", which is weaker than S256 and is\n    an Auth0 tenant default rather than a deliberate Textla choice.\n- id: implicit-grant-enabled\n  value: true\n  evidence: >-\n    grant_types_supported includes \"implicit\" and \"password\" — both discouraged by OAuth 2.1.\n    Again an Auth0 tenant default, not evidence of a Textla design decision.\n- id: dpop-supported\n  value: true\n  evidence: dpop_signing_alg_values_supported includes ES256.\n- id: mtls\n  value: false\n  evidence: No mutualTLS or tls_client_auth advertised in the discovery document.\nscopes_advertised:\n\
  - openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\nbyoc_credentials:\n  note: >-\n    Textla's only documented credential flow for customers is BYOC (bring your own carrier):\n    the help center walks a customer through connecting their own Twilio account to Textla.\n    Those are Twilio credentials held by the customer, not a Textla API credential.\n  docs: https://help.textla.com/en/collections/3372927-docs-for-byoc\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textla-inc/refs/heads/main/authentication/textla-inc-authentication.yml
summary_line: 0 schemes
tags:
- Company
- SMS
- Text Messaging
- Business Messaging
- Bulk SMS
- Communications
- Marketing
- Customer Engagement
---
