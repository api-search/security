---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Equipmentshare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: EquipmentShare secures its APIs with oauth2, apiKey, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: EquipmentShare
provider_slug: equipmentshare
scheme_count: 3
schemes:
- claims:
    uid: https://es-erp/uid
    workspace: workspace_id
  description: 'User-delegated access. The user signs in via T3OS, selects a workspace at the consent screen, and the app receives a Bearer access token scoped to that user. Authorization Code + PKCE, no client SDK required. Sent as `Authorization: Bearer <token>` to the GraphQL API.'
  flows:
  - audience: https://api.equipmentshare.com/es-erp-api/delegated
    authorizationUrl: https://equipmentshare-erp.us.auth0.com/authorize
    flow: authorizationCode
    logoutUrl: https://equipmentshare-erp.us.auth0.com/v2/logout
    pkce: true
    tokenUrl: https://equipmentshare-erp.us.auth0.com/oauth/token
  name: T3OS OAuth2 (user-delegated)
  sources:
  - https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world
  type: oauth2
- description: Unattended, workspace-scoped access for syncs, exports, scheduled jobs and webhooks. A workspace admin installs the app once (installWorkspaceApp); T3OS mints a principal, creates a workspace-scoped API key, and signs an install-token JWT delivered to the app's installCallbackUrl. The JWT is verified against the es-erp-api JWKS; the API key is then sent as `X-API-Key` on GraphQL calls. Keys do not expire and are invalidated only on uninstall.
  in: header
  install_token:
    issuer: https://api.equipmentshare.com/es-erp-api
    jwks_uri: https://api.equipmentshare.com/es-erp-api/.well-known/jwks.json
  name: T3OS Workspace-installed API Key
  parameter_name: X-API-Key
  sources:
  - https://github.com/EquipmentShare/t3os-examples/tree/main/apps/workspace-hello-world
  type: apiKey
- description: Pure "Sign in with T3OS" identity — no workspace selection, no API access. T3OS acts as an OIDC identity provider; the third-party app keys its own user table off the `https://es-erp/uid` claim.
  name: T3OS OpenID Connect (sign-in only)
  openIdConnectUrl: https://equipmentshare-erp.us.auth0.com/.well-known/openid-configuration
  sources:
  - https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oidc-hello-world
  type: openIdConnect
slug: equipmentshare-authentication
source_filename: equipmentshare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/EquipmentShare/t3os-examples\ndocs: https://github.com/EquipmentShare/t3os-examples\n# T3OS (the EquipmentShare developer platform, es-erp-api) publishes three first-party auth\n# flows, documented end-to-end in the MIT-licensed t3os-examples reference apps and backed by\n# a production Auth0 tenant. Verified live: the Auth0 OIDC discovery document and the es-erp-api\n# JWKS endpoint both return 200 (see well-known/).\nsummary:\n  types: [oauth2, apiKey, openIdConnect]\n  api_key_in: [header]\n  api_key_header: X-API-Key\n  oauth2_flows: [authorizationCode]\n  pkce: required\n  identity_provider: Auth0\n  auth0_tenant: equipmentshare-erp.us.auth0.com\n  auth0_tenant_staging: staging-equipmentshare-erp.us.auth0.com\nschemes:\n- name: T3OS OAuth2 (user-delegated)\n  type: oauth2\n  description: >-\n    User-delegated access. The user signs in via T3OS, selects a workspace at the consent\n    screen, and the\
  \ app receives a Bearer access token scoped to that user. Authorization Code\n    + PKCE, no client SDK required. Sent as `Authorization: Bearer <token>` to the GraphQL API.\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://equipmentshare-erp.us.auth0.com/authorize\n    tokenUrl: https://equipmentshare-erp.us.auth0.com/oauth/token\n    logoutUrl: https://equipmentshare-erp.us.auth0.com/v2/logout\n    audience: https://api.equipmentshare.com/es-erp-api/delegated\n  claims:\n    uid: https://es-erp/uid\n    workspace: workspace_id\n  sources: [https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world]\n- name: T3OS Workspace-installed API Key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    Unattended, workspace-scoped access for syncs, exports, scheduled jobs and webhooks. A\n    workspace admin installs the app once (installWorkspaceApp); T3OS mints a principal, creates\n    a workspace-scoped\
  \ API key, and signs an install-token JWT delivered to the app's\n    installCallbackUrl. The JWT is verified against the es-erp-api JWKS; the API key is then sent\n    as `X-API-Key` on GraphQL calls. Keys do not expire and are invalidated only on uninstall.\n  install_token:\n    issuer: https://api.equipmentshare.com/es-erp-api\n    jwks_uri: https://api.equipmentshare.com/es-erp-api/.well-known/jwks.json\n  sources: [https://github.com/EquipmentShare/t3os-examples/tree/main/apps/workspace-hello-world]\n- name: T3OS OpenID Connect (sign-in only)\n  type: openIdConnect\n  openIdConnectUrl: https://equipmentshare-erp.us.auth0.com/.well-known/openid-configuration\n  description: >-\n    Pure \"Sign in with T3OS\" identity — no workspace selection, no API access. T3OS acts as an\n    OIDC identity provider; the third-party app keys its own user table off the\n    `https://es-erp/uid` claim.\n  sources: [https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oidc-hello-world]\nnotes:\
  \ >-\n  App registration/lifecycle is managed through T3OS management operations (registerApp,\n  updateApp, installWorkspaceApp) and the T3OS dev portal at https://app.t3os.ai, where\n  clientSecret and workspace API keys can be rotated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipmentshare/refs/heads/main/authentication/equipmentshare-authentication.yml
summary_line: oauth2/apiKey/openIdConnect · 3 schemes
tags:
- Company
- Construction Technology
- Fleet Management
- Telematics
- Equipment Rental
- GraphQL
- Developer Platform
- OAuth
---
