---
anonymous_access: false
api_key_in: []
api_specs:
- filename: green-screens-ai-prediction-api-openapi.yml
  format: yaml
  label: Green Screens AI Prediction API
  slug: green-screens-ai-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-prediction-api-openapi.yml
- filename: green-screens-ai-auth-api-openapi.yml
  format: yaml
  label: Green Screens AI Auth API
  slug: green-screens-ai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-auth-api-openapi.yml
- filename: green-screens-ai-analytics-api-openapi.yml
  format: yaml
  label: Green Screens AI Analytics API
  slug: green-screens-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-analytics-api-openapi.yml
- filename: green-screens-ai-bids-api-openapi.yml
  format: yaml
  label: Green Screens AI Bids API
  slug: green-screens-ai-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-bids-api-openapi.yml
- filename: green-screens-ai-history-api-openapi.yml
  format: yaml
  label: Green Screens AI History API
  slug: green-screens-ai-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-history-api-openapi.yml
- filename: green-screens-ai-pricing-api-openapi.yml
  format: yaml
  label: Green Screens AI Pricing API
  slug: green-screens-ai-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-pricing-api-openapi.yml
- filename: green-screens-ai-quotes-api-openapi.yml
  format: yaml
  label: Green Screens AI Quotes API
  slug: green-screens-ai-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-quotes-api-openapi.yml
- filename: green-screens-ai-tms-api-openapi.yml
  format: yaml
  label: Green Screens AI TMS API
  slug: green-screens-ai-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-tms-api-openapi.yml
- filename: green-screens-ai-market-intelligence-api-openapi.yml
  format: yaml
  label: Green Screens AI Market Intelligence API
  slug: green-screens-ai-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-market-intelligence-api-openapi.yml
auth_types:
- oauth2
- http
description: Two-step authentication. Exchange a provider-issued client_id and client_secret for a JWT at the OAuth2 token endpoint, then present it as a bearer token on every other operation. The identity provider is Keycloak.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Green Screens Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Green Screens AI secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Green Screens AI
provider_slug: green-screens-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'The scheme every service spec declares. Access token from POST /auth/token, presented as Authorization: Bearer <access_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/green-screens-ai-analytics-api-openapi.yml
  - openapi/green-screens-ai-auth-api-openapi.yml
  - openapi/green-screens-ai-bids-api-openapi.yml
  - openapi/green-screens-ai-datalake-api-openapi.yml
  - openapi/green-screens-ai-history-api-openapi.yml
  - openapi/green-screens-ai-marketintelligence-api-openapi.yml
  - openapi/green-screens-ai-prediction-api-openapi.yml
  - openapi/green-screens-ai-prediction-v2-api-openapi.yml
  - openapi/green-screens-ai-pricing-api-openapi.yml
  - openapi/green-screens-ai-quotes-api-openapi.yml
  - openapi/green-screens-ai-quotes-v1-api-openapi.yml
  - openapi/green-screens-ai-tms-api-openapi.yml
  type: http
- alternateTokenUrls:
  - https://intelligence.triumph.io/v1/auth/token
  - https://betaapi.greenscreens.ai/v1/auth/token
  - https://testapi.greenscreens.ai/v1/auth/token
  description: Documented by the provider as an operation (POST /auth/token) rather than declared as an oauth2 securityScheme object, which is why the spec-only derivation sees http/bearer and not oauth2. The flow is a conformant RFC 6749 client_credentials grant.
  flow: clientCredentials
  name: oauth2ClientCredentials
  probed:
    body: '{"error":"invalid_request","error_description":"Missing form parameter: grant_type"}'
    date: '2026-09-12'
    method: POST
    status: 400
    url: https://api.greenscreens.ai/v1/auth/token
  request:
    media_type: application/x-www-form-urlencoded
    parameters:
    - grant_type (must be client_credentials)
    - client_id
    - client_secret
  response:
    fields:
    - access_token
    - expires_in
    - refresh_expires_in
    - token_type
    - not-before-policy
    - scope
  scopes: []
  scopes_note: The token response carries a scope string, but the provider publishes no scope reference and no operation declares required scopes. Entitlement is enforced by Keycloak ROLES granted per account (the provider's release notes gate RFP Manager on "a Keycloak role"), not by caller-requested scopes — so there is no scopes artifact to write. 403 access_forbidden is the runtime signal that an account lacks a feature.
  tokenUrl: https://api.greenscreens.ai/v1/auth/token
  type: oauth2
slug: green-screens-ai-authentication
source_filename: green-screens-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  securitySchemes of the provider's 12 published OpenAPI documents\n  (https://connect.greenscreens.ai/<service>/<version>/openapi.yaml), the verbatim /auth/token\n  operation in https://connect.greenscreens.ai/openapi.yaml, and the provider's own help-center\n  articles https://intelligencehelp.triumph.io/en/articles/10684487-managing-api-credentials and\n  https://intelligencehelp.triumph.io/en/articles/12461044-acquiring-the-access-token-for-triumph-intelligence-apis\ndocs: https://intelligencehelp.triumph.io/en/articles/12461044-acquiring-the-access-token-for-triumph-intelligence-apis\nprovider: Green Screens AI\nproviderId: green-screens-ai\ndescription: >-\n  Two-step authentication. Exchange a provider-issued client_id and client_secret for a JWT at the\n  OAuth2 token endpoint, then present it as a bearer token on every other operation. The identity\n  provider is Keycloak.\nsummary:\n  types:\n  - oauth2\n  - http\n\
  \  self_serve: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    The scheme every service spec declares. Access token from POST /auth/token, presented as\n    Authorization: Bearer <access_token>.\n  sources:\n  - openapi/green-screens-ai-analytics-api-openapi.yml\n  - openapi/green-screens-ai-auth-api-openapi.yml\n  - openapi/green-screens-ai-bids-api-openapi.yml\n  - openapi/green-screens-ai-datalake-api-openapi.yml\n  - openapi/green-screens-ai-history-api-openapi.yml\n  - openapi/green-screens-ai-marketintelligence-api-openapi.yml\n  - openapi/green-screens-ai-prediction-api-openapi.yml\n  - openapi/green-screens-ai-prediction-v2-api-openapi.yml\n  - openapi/green-screens-ai-pricing-api-openapi.yml\n  - openapi/green-screens-ai-quotes-api-openapi.yml\n  - openapi/green-screens-ai-quotes-v1-api-openapi.yml\n  - openapi/green-screens-ai-tms-api-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n\
  \  description: >-\n    Documented by the provider as an operation (POST /auth/token) rather than declared as an oauth2\n    securityScheme object, which is why the spec-only derivation sees http/bearer and not oauth2. The\n    flow is a conformant RFC 6749 client_credentials grant.\n  tokenUrl: https://api.greenscreens.ai/v1/auth/token\n  alternateTokenUrls:\n  - https://intelligence.triumph.io/v1/auth/token\n  - https://betaapi.greenscreens.ai/v1/auth/token\n  - https://testapi.greenscreens.ai/v1/auth/token\n  request:\n    media_type: application/x-www-form-urlencoded\n    parameters:\n    - grant_type (must be client_credentials)\n    - client_id\n    - client_secret\n  response:\n    fields:\n    - access_token\n    - expires_in\n    - refresh_expires_in\n    - token_type\n    - not-before-policy\n    - scope\n  scopes: []\n  scopes_note: >-\n    The token response carries a scope string, but the provider publishes no scope reference and no\n    operation declares required scopes.\
  \ Entitlement is enforced by Keycloak ROLES granted per account\n    (the provider's release notes gate RFP Manager on \"a Keycloak role\"), not by caller-requested\n    scopes — so there is no scopes artifact to write. 403 access_forbidden is the runtime signal that\n    an account lacks a feature.\n  probed:\n    url: https://api.greenscreens.ai/v1/auth/token\n    method: POST\n    status: 400\n    body: '{\"error\":\"invalid_request\",\"error_description\":\"Missing form parameter: grant_type\"}'\n    date: '2026-09-12'\nprovisioning:\n  self_serve: false\n  path: >-\n    Credentials are created inside the Triumph Intelligence application: Profile icon > Preferences >\n    Credentials. Only Admin users can see the tab. Each credential set has a Client ID (auto-generated),\n    a Client Secret (auto-generated, viewable/copyable), a Description, and an enabled/disabled Status.\n  provider_guidance: >-\n    The provider explicitly recommends one credential set per integration so a single\
  \ partner can be\n    disabled or deleted without revoking the others, and warns that a shared credential set cannot be\n    revoked per-partner later.\n  rotation: >-\n    Credentials can be disabled without deletion, and a new set can be generated at any time. No\n    automatic expiry or forced-rotation policy is published.\nbrowser_use:\n  supported: conditional\n  note: >-\n    For browser callers the provider documents a back-end wrapper: your own server calls /v1/auth/token\n    with the client credentials and proxies only the access_token to the front end, behind your own\n    authentication. A Google id_token path (gauth) also exists but must be enabled per application by\n    the provider on request. Your origins must additionally be added to the provider's CORS allowlist.\n  source: https://intelligencehelp.triumph.io/en/articles/12461044-acquiring-the-access-token-for-triumph-intelligence-apis\nruntime_evidence:\n- url: https://api.greenscreens.ai/v3/prediction/rates\n  method:\
  \ POST\n  status: 401\n  header: 'WWW-Authenticate: Bearer'\n  date: '2026-09-12'\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/authentication/green-screens-ai-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Artificial Intelligence
- Freight
- Logistics
- Machine-Learning
- Pricing
- Transportation
---
