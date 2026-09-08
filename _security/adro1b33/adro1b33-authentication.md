---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adro1b33-aox-openapi.yaml
  format: yaml
  label: AOX Platform API
  slug: aox-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/openapi/adro1b33-aox-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Adro1B33 Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADRO declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ADRO
provider_slug: adro1b33
scheme_count: 0
schemes: []
slug: adro1b33-authentication
source_filename: adro1b33-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: >-\n  openapi/adro1b33-aox-openapi.yaml (no components.securitySchemes are declared, so the model below is\n  derived from the account operations and their request/response schemas) plus live anonymous probes of\n  api.aoxlabs.com recorded under evidence[], and well-known/adro1b33-openid-configuration.json for the\n  separate storefront identity surface.\napis:\n- api: AOX Platform API\n  host: https://api.aoxlabs.com\n  declared_security_schemes: []\n  gap: >-\n    THE SPEC DECLARES NO securitySchemes AND NO GLOBAL security BLOCK. drf-spectacular emitted the\n    document without an authentication configuration, so a consumer reading the contract alone cannot\n    tell how to authenticate. 212 of 231 operations carry no security field at all and 19 carry\n    `security: [{}]`, which marks them explicitly public. The real behaviour has to be probed.\n  observed_model:\n    style: session\n    mechanism: >-\n      Credential\
  \ exchange at POST /accounts/login/ (email + password) and POST /accounts/social-login/,\n      with POST /accounts/token/refresh/ for renewal and POST /accounts/logout/ to end the session. The\n      LoginResponse schema carries no token field (only detail, teamId, teamName, userType,\n      mustChangePassword), which is consistent with a browser-oriented httpOnly cookie session rather\n      than a bearer token handed to the client.\n    bearer_token_documented: false\n    api_key_documented: false\n    confidence: medium\n    note: >-\n      No published developer documentation describes machine-to-machine authentication for this API.\n      This is the honest limit of what can be established anonymously; the exact credential material\n      cannot be confirmed without an account.\n  multi_tenancy:\n    model: team\n    mechanism: >-\n      Every substantive resource is scoped to a team. POST /accounts/team-switch/ changes the active\n      team for the session, GET /accounts/teams/\
  \ lists memberships, and Project, Job, CreditWallet,\n      Subscription and Payment all carry teamId. POST /tenants/exists/ is a public tenant-existence\n      check.\n  public_operations:\n    count: 19\n    operations:\n    - accounts_login_create\n    - accounts_logout_create\n    - accounts_signup_create\n    - accounts_social_login_create\n    - accounts_social_register_create\n    - accounts_token_refresh_create\n    - accounts_password_reset_create\n    - accounts_password_reset_confirm_create\n    - board_retrieve\n    - board_retrieve_2\n    - book_demo_create\n    - credits_bundles_list\n    - credits_bundles_retrieve\n    - health_retrieve\n    - plans_list\n    - plans_retrieve\n    - tenants_exists_create\n    - verifier_email_verifier_create\n    - verifier_email_verifier_confirm_create\n  password_policy_surface:\n  - PUT /accounts/me/password-change/\n  - POST /accounts/me/password-verify/\n  - POST /accounts/me/force-password-change/\n  - POST /accounts/password-reset/\n\
  \  - POST /accounts/password-reset-confirm/\n  evidence:\n  - url: https://api.aoxlabs.com/\n    status: 401\n    body: '{\"detail\":\"자격 인증 데이터가 제공되지 않았습니다.\"}'\n    note: Django REST Framework \"Authentication credentials were not provided\" (Korean locale).\n  - url: https://api.aoxlabs.com/announcements/\n    status: 401\n  - url: https://api.aoxlabs.com/board/\n    status: 200\n    note: >-\n      Confirms the spec's `security: [{}]` marking — this operation really is anonymous.\n  - url: https://api.aoxlabs.com/health/\n    status: 200\n    body: '{\"status\":\"ok\"}'\n  - url: https://api.aoxlabs.com/schema/\n    status: 200\n    note: The OpenAPI document itself is served anonymously.\n- api: ADRO US Store Agent Commerce (UCP / MCP)\n  host: https://adro.com\n  observed_model:\n    style: oidc\n    mechanism: >-\n      Shopify Customer Accounts. adro.com serves OpenID Connect and OAuth 2.0 authorization-server\n      metadata on its own domain, issued for ADRO's shop (issuer\n\
  \      https://shopify.com/authentication/67310649500). Authorization code with PKCE (S256), refresh\n      tokens and the JWT bearer grant; RS256 id tokens; bearer methods: header.\n    confidence: high\n  anonymous_surface: >-\n    The UCP MCP endpoint at POST /api/ucp/mcp answers tools/list with no credential at all. Catalog\n    browsing, cart and checkout creation are anonymous; only payment completion requires buyer consent.\n  scopes: scopes/adro1b33-scopes.yml\n  evidence:\n  - url: https://adro.com/.well-known/openid-configuration\n    status: 200\n  - url: https://adro.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://shopify.com/authentication/67310649500/.well-known/jwks.json\n    status: 200\n  - url: https://adro.com/api/ucp/mcp\n    status: 200\n    note: POST tools/list, no Authorization header sent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/authentication/adro1b33-authentication.yml
summary_line: 0 schemes
tags:
- Aerodynamics
- Computational Fluid Dynamics
- Simulation
- Automotive
- Engineering
- Optimization
- Manufacturing
- Artificial Intelligence
- High Performance Computing
- Ecommerce
- MCP
- South Korea
---
