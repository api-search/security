---
api_key_in: []
auth_types:
- oauth2
- publicKey
description: ''
kind: authentication
layout: security
method: searched
name: Wealthcom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wealth.com secures its APIs with oauth2 and publicKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wealth.com
provider_slug: wealthcom
scheme_count: 3
schemes:
- api: Wealth.com Advisor API
  base_url: https://advisor-api.wealth.com/v1
  flow: authorizationCode
  name: AdvisorOAuth2
  pkce:
    challenge_method: S256
    note: PKCE recommended; may be required for public clients (SPAs, native apps).
    supported: true
  scopes:
    note: Standard OpenID Connect scopes plus any custom configured scopes.
    standard:
    - openid
    - email
    - profile
  token:
    access_token_ttl: ~1 hour
    algorithm: RS256
    format: JWT
    header: 'Authorization: Bearer <access_token>'
    refresh_token_ttl: up to ~30 days (environment dependent)
    type: bearer
    validation:
    - Token must be a JWT access token (ID tokens are rejected for API calls).
    - Must contain iss and sub claims and must not be expired.
    - kid header verified against the authorization server's JWKS.
  type: oauth2
- api: Wealth.com Onboarding API
  docs: https://developer.wealth.com/onboarding/authentication
  mechanism: RSA public/private key pair
  name: OnboardingPublicKey
  note: Partners generate an RSA key pair, export the public key to a .pem file, and share it with Wealth.com. Connections encrypted using TLS 1.2 or higher.
  type: publicKey
- api: Wealth.com Advisor API (webhooks)
  in: header
  name: WebhookApiKey
  note: Each webhook POST includes a wealth-api-key header that the receiver validates against the Wealth.com-issued API key (UUID). Keys may be rotated by Wealth.com.
  parameter_name: wealth-api-key
  type: apiKey
slug: wealthcom-authentication
source_filename: wealthcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wealth.com/advisor/authentication\ndocs: https://developer.wealth.com/advisor/authentication\nsummary:\n  types: [oauth2, publicKey]\n  oauth2_flows: [authorizationCode]\n  pkce: recommended-required-for-public-clients\n  token_format: JWT (RS256, asymmetric, verified against authorization-server JWKS)\n  transport_security: TLS 1.2 or higher required\nschemes:\n- name: AdvisorOAuth2\n  api: Wealth.com Advisor API\n  type: oauth2\n  flow: authorizationCode\n  pkce:\n    supported: true\n    challenge_method: S256\n    note: PKCE recommended; may be required for public clients (SPAs, native apps).\n  token:\n    type: bearer\n    header: 'Authorization: Bearer <access_token>'\n    format: JWT\n    algorithm: RS256\n    validation:\n      - Token must be a JWT access token (ID tokens are rejected for API calls).\n      - Must contain iss and sub claims and must not be expired.\n      - kid header verified against\
  \ the authorization server's JWKS.\n    access_token_ttl: ~1 hour\n    refresh_token_ttl: up to ~30 days (environment dependent)\n  scopes:\n    standard: [openid, email, profile]\n    note: Standard OpenID Connect scopes plus any custom configured scopes.\n  base_url: https://advisor-api.wealth.com/v1\n- name: OnboardingPublicKey\n  api: Wealth.com Onboarding API\n  type: publicKey\n  mechanism: RSA public/private key pair\n  docs: https://developer.wealth.com/onboarding/authentication\n  note: >-\n    Partners generate an RSA key pair, export the public key to a .pem file, and share it\n    with Wealth.com. Connections encrypted using TLS 1.2 or higher.\n- name: WebhookApiKey\n  api: Wealth.com Advisor API (webhooks)\n  type: apiKey\n  in: header\n  parameter_name: wealth-api-key\n  note: >-\n    Each webhook POST includes a wealth-api-key header that the receiver validates against\n    the Wealth.com-issued API key (UUID). Keys may be rotated by Wealth.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthcom/refs/heads/main/authentication/wealthcom-authentication.yml
summary_line: oauth2/publicKey · 3 schemes
tags:
- Company
- Enterprise
- Estate Planning
- Tax Planning
- Wealth Management
- Financial Advisors
- Fintech
- Artificial Intelligence
---
