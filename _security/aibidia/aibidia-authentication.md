---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aibidia-aibidia-tp-ai-api-api-openapi.yml
  format: yaml
  label: Aibidia Aibidia TP AI API
  slug: aibidia-aibidia-tp-ai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-aibidia-tp-ai-api-api-openapi.yml
- filename: aibidia-authorize-api-openapi.yml
  format: yaml
  label: Aibidia Authorize API
  slug: aibidia-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-authorize-api-openapi.yml
- filename: aibidia-create-session-api-openapi.yml
  format: yaml
  label: Aibidia Create Session API
  slug: aibidia-create-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-create-session-api-openapi.yml
- filename: aibidia-datainjections-api-openapi.yml
  format: yaml
  label: Aibidia Data Injections API
  slug: aibidia-datainjections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-datainjections-api-openapi.yml
- filename: aibidia-extracttypes-api-openapi.yml
  format: yaml
  label: Aibidia Extract Types API
  slug: aibidia-extracttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-extracttypes-api-openapi.yml
- filename: aibidia-health-api-openapi.yml
  format: yaml
  label: Aibidia Health API
  slug: aibidia-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-health-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aibidia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aibidia secures its APIs with apiKey, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aibidia
provider_slug: aibidia
scheme_count: 2
schemes:
- applies_to:
  - https://otpm-api.aibidia.com/api/datainjections/automated
  - https://otpm-api.aibidia.com/api/extract-types/integration
  description: API key authentication for the Public OTP Management API. The key is bound to a single Extract Type — the GET /api/extract-types/integration operation returns "the configuration and current status of extracts for the Extract Type associated with the provided API key" — so the credential itself carries the scope and no identifier is passed in the request. Keys are provisioned by Aibidia to an existing customer; there is no public self-serve issuance path.
  in: header
  name: X-DATAINGESTION-API-KEY
  parameter: X-DATAINGESTION-API-KEY
  sources:
  - openapi/aibidia-otp-management-public-openapi.yml
  type: apiKey
- authorization_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/authorize
  description: Interactive sign-in for platform.aibidia.com and every solution module (TPDoc, CbCR, OTPM, STPM, VCA, Data Studio, Horizon, TP AI). Microsoft Entra External ID / Azure AD B2C on Aibidia's own custom domain, driven by MSAL in the browser. The TP Aurora product is a separate B2C tenant (tpauroraprod.b2clogin.com) rather than part of the auth.aibidia.com estate.
  end_session_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/logout
  flow: authorization_code
  id_token_signing_alg: RS256
  identity_providers:
    note: The platform ships a SHOW_IDENTITY_PROVIDER feature flag set true in production, and the B2C policy advertises "idp" and "authenticationSource" claims, so federated enterprise identity providers are in play. Which providers are federated is not published anonymously.
  issuer: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/v2.0/
  jwks_uri: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/discovery/v2.0/keys
  name: Azure AD B2C (MSAL)
  openid_configuration: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/B2C_1A_SUSI/v2.0/.well-known/openid-configuration
  policy: B2C_1A_SUSI
  resource_scope: https://auth.aibidia.com/AibidiaAPI/user_impersonation
  scopes_supported_in_discovery:
  - openid
  sources:
  - https://platform.aibidia.com/env.js
  - https://platform.aibidia.com/tpai/env.js
  - well-known/aibidia-openid-configuration.json
  subject_types: pairwise
  token_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/token
  type: openIdConnect
slug: aibidia-authentication
source_filename: aibidia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  openapi/aibidia-otp-management-public-openapi.yml (served by Aibidia at\n  https://otpm-api.aibidia.com/swagger/public/swagger.json) plus Aibidia's own published platform runtime\n  configuration at https://platform.aibidia.com/env.js and https://platform.aibidia.com/tpai/env.js, and the\n  Azure AD B2C OpenID Provider Metadata saved at well-known/aibidia-openid-configuration.json.\ndocs: https://otpm-api.aibidia.com/swagger/index.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  note: >-\n    Aibidia runs two distinct authentication regimes. Machine-to-machine integration with the public OTP\n    Management data-ingestion surface uses a per-Extract-Type API key in a request header. Every interactive\n    platform solution instead uses Azure AD B2C (custom domain auth.aibidia.com) through MSAL, exchanging an\n    OIDC authorization code for an access token scoped to a single\
  \ resource scope.\nschemes:\n- name: X-DATAINGESTION-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-DATAINGESTION-API-KEY\n  description: >-\n    API key authentication for the Public OTP Management API. The key is bound to a single Extract Type — the\n    GET /api/extract-types/integration operation returns \"the configuration and current status of extracts for\n    the Extract Type associated with the provided API key\" — so the credential itself carries the scope and no\n    identifier is passed in the request. Keys are provisioned by Aibidia to an existing customer; there is no\n    public self-serve issuance path.\n  applies_to:\n  - https://otpm-api.aibidia.com/api/datainjections/automated\n  - https://otpm-api.aibidia.com/api/extract-types/integration\n  sources:\n  - openapi/aibidia-otp-management-public-openapi.yml\n- name: Azure AD B2C (MSAL)\n  type: openIdConnect\n  flow: authorization_code\n  description: >-\n    Interactive sign-in for platform.aibidia.com and every\
  \ solution module (TPDoc, CbCR, OTPM, STPM, VCA, Data\n    Studio, Horizon, TP AI). Microsoft Entra External ID / Azure AD B2C on Aibidia's own custom domain, driven by\n    MSAL in the browser. The TP Aurora product is a separate B2C tenant (tpauroraprod.b2clogin.com) rather than\n    part of the auth.aibidia.com estate.\n  openid_configuration: >-\n    https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/B2C_1A_SUSI/v2.0/.well-known/openid-configuration\n  issuer: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/v2.0/\n  authorization_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/authorize\n  token_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/token\n  jwks_uri: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/discovery/v2.0/keys\n  end_session_endpoint: https://auth.aibidia.com/087223a3-c05b-420d-b854-db9b237f5a71/b2c_1a_susi/oauth2/v2.0/logout\n\
  \  policy: B2C_1A_SUSI\n  id_token_signing_alg: RS256\n  subject_types: pairwise\n  resource_scope: https://auth.aibidia.com/AibidiaAPI/user_impersonation\n  scopes_supported_in_discovery:\n  - openid\n  identity_providers:\n    note: >-\n      The platform ships a SHOW_IDENTITY_PROVIDER feature flag set true in production, and the B2C policy\n      advertises \"idp\" and \"authenticationSource\" claims, so federated enterprise identity providers are in\n      play. Which providers are federated is not published anonymously.\n  sources:\n  - https://platform.aibidia.com/env.js\n  - https://platform.aibidia.com/tpai/env.js\n  - well-known/aibidia-openid-configuration.json\ngaps:\n- >-\n  No published authentication reference page. The Public OTP Management API's only documentation is the Swagger\n  UI it serves itself; how an integrator obtains an X-DATAINGESTION-API-KEY is not stated anywhere anonymously\n  reachable.\n- >-\n  The B2C discovery document advertises scopes_supported as [\"\
  openid\"] only, while the platform actually requests\n  https://auth.aibidia.com/AibidiaAPI/user_impersonation. A client reading discovery alone cannot learn the\n  resource scope it needs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/authentication/aibidia-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Transfer Pricing
- Tax Technology
- Tax Compliance
- Regulatory Reporting
- Country-by-Country Reporting
- Financial Data
- Enterprise Software
- Data Ingestion
- Finland
---
