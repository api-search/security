---
api_key_in:
- header
api_specs:
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE API
  slug: vaultre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE Integrator API
  slug: vaultre-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-aggregator-api-v1-0-openapi.yml
  format: yaml
  label: VaultRE Aggregator API
  slug: vaultre-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-aggregator-api-v1-0-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vaultre Authentication
name_suffix: Authentication
oauth_flows: []
overview: VaultRE secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VaultRE
provider_slug: vaultre
scheme_count: 4
schemes:
- description: Integrator API key. Identifies the integrator to VaultRE, issued only after an integration request is reviewed and approved. Must be kept secret and not shared.
  failure: HTTP 403 Forbidden when missing or invalid.
  in: header
  name: Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/vaultre-api-v1-1-openapi.yml
  - openapi/vaultre-api-v1-2-openapi.yml
  - openapi/vaultre-api-v1-3-openapi.yml
  type: apiKey
- description: Aggregator variant. "This value is provided to you by VaultRE and identifies you as a CRM" — the aggregator's Secret Key rather than the core integrator key.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/vaultre-aggregator-api-v1-0-openapi.yml
  type: apiKey
- description: 'Customer access token on the core API; HS512 JWT on integrator and aggregator endpoints. The aggregator spec states: "This value is a JWT token signed with the HS512 algorithm using your X-Api-Key value as the secret."'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/vaultre-api-v1-3-openapi.yml
  - openapi/vaultre-aggregator-api-v1-0-openapi.yml
  type: http
- description: Use format 'Bearer [token]'. Modelled as an apiKey header in the older specs.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/vaultre-api-v1-1-openapi.yml
  - openapi/vaultre-api-v1-2-openapi.yml
  type: apiKey
slug: vaultre-authentication
source_filename: vaultre-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://docs.api.vaultre.com.au/guide.html (upgraded from a derived pass over\n  openapi/vaultre-api-v1-1-openapi.yml, openapi/vaultre-api-v1-2-openapi.yml,\n  openapi/vaultre-api-v1-3-openapi.yml, openapi/vaultre-aggregator-api-v1-0-openapi.yml)\ndocs:\n- https://docs.api.vaultre.com.au/guide.html\n- https://docs.api.vaultre.com.au/basics.html\n- https://docs.api.vaultre.com.au/oauth.html\n- https://docs.api.vaultre.com.au/integrator.html\n- https://docs.api.vaultre.com.au/aggregator.html\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: >-\n    Every request carries TWO credentials: an integrator-level API key in X-Api-Key and\n    a bearer token in Authorization. Which bearer token depends on the surface — a\n    customer-granted access token for the core API, or a short-lived self-signed HS512\n    JWT for integrator-level and Aggregator endpoints. Neither credential is self-serve:\n\
  \    the key requires integrator approval, the customer token requires the agency to\n    grant it.\n  gate: approval + per-account customer consent\nschemes:\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Integrator API key. Identifies the integrator to VaultRE, issued only after an\n    integration request is reviewed and approved. Must be kept secret and not shared.\n  failure: HTTP 403 Forbidden when missing or invalid.\n  sources:\n  - openapi/vaultre-api-v1-1-openapi.yml\n  - openapi/vaultre-api-v1-2-openapi.yml\n  - openapi/vaultre-api-v1-3-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Aggregator variant. \"This value is provided to you by VaultRE and identifies you as\n    a CRM\" — the aggregator's Secret Key rather than the core integrator key.\n  sources:\n  - openapi/vaultre-aggregator-api-v1-0-openapi.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  description:\
  \ >-\n    Customer access token on the core API; HS512 JWT on integrator and aggregator\n    endpoints. The aggregator spec states: \"This value is a JWT token signed with the\n    HS512 algorithm using your X-Api-Key value as the secret.\"\n  sources:\n  - openapi/vaultre-api-v1-3-openapi.yml\n  - openapi/vaultre-aggregator-api-v1-0-openapi.yml\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"Use format 'Bearer [token]'. Modelled as an apiKey header in the older specs.\"\n  sources:\n  - openapi/vaultre-api-v1-1-openapi.yml\n  - openapi/vaultre-api-v1-2-openapi.yml\nsurfaces:\n- surface: core API\n  base_url: https://ap-southeast-2.api.vaultre.com.au/api/v1.3\n  headers:\n  - 'X-Api-Key: <integrator API key>'\n  - 'Authorization: Bearer <customer access token>'\n  token_source: >-\n    Issued by the customer from Office Integrations > Third-Party Access > Create Token,\n    or generated through the OAuth flow. Scoped by the customer and revocable\
  \ at any\n    time. One token per customer account.\n  scopes_readable_at: GET /scopes (operationId getTokenScopes)\n- surface: integrator endpoints\n  base_url: https://ap-southeast-2.api.vaultre.com.au/api/v1.3/integrator\n  headers:\n  - 'X-Api-Key: <integrator API key>'\n  - 'Authorization: Bearer <self-signed JWT>'\n  jwt:\n    algorithm: HS512\n    payload: '{\"apiKey\": \"<your API key>\", \"timestamp\": <current epoch seconds>}'\n    secret: secret key provided by VaultRE\n    ttl_seconds: 300\n  sample_code: https://github.com/VaultGroup/api-samples/blob/master/python/create_jwt.py\n- surface: Aggregator API\n  base_url: https://aggregator.api.vaultre.com.au/api/v1.0\n  headers:\n  - 'X-Api-Key: <Secret Key>'\n  - 'Authorization: Bearer <self-signed JWT>'\n  jwt:\n    algorithm: HS512\n    payload: '{\"crmKey\": \"<your provided CRM key>\", \"timestamp\": <current epoch seconds>}'\n    secret: secret key provided by VaultRE\n    ttl_seconds: 120\n  note: Registration for Aggregator\
  \ access is separate from core API integrator registration.\n  sample_code: https://github.com/VaultGroup/api-samples/blob/master/aggregator/client.py\n- surface: webhooks (inbound to the integrator)\n  authentication: >-\n    None. VaultRE states webhook requests \"are not sent with any other form of\n    authentication or authorisation\" — the receiving endpoint must accept unauthenticated\n    requests and verify the X-VaultRE-Signature HMAC-SHA512 header instead.\n  artifact: asyncapi/vaultre-webhooks.yml\ntoken_minting:\n  manual: Customer creates the token inside their VaultRE account and hands it to the developer.\n  oauth: >-\n    OAuth2-style authorization-code flow for minting customer tokens without handling\n    VaultRE credentials — see scopes/vaultre-scopes.yml for endpoints, the 60-second\n    code TTL and the literal redirect-URI matching rule.\n  artifact: scopes/vaultre-scopes.yml\ndiscovery:\n  openid_configuration: absent (404 on login.vaultre.com.au and the API host)\n\
  \  oauth_authorization_server_metadata: absent (404)\n  dynamic_client_registration: not supported\n  artifact: well-known/vaultre-well-known.yml\ncontact: api@vaultre.com.au\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/authentication/vaultre-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Real Estate
- Australia
- New Zealand
- PropTech
- CRM
- Property Listings
- Property Management
- Rentals
- Commercial Real Estate
- Webhooks
---
