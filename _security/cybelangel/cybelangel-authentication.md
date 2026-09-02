---
api_key_in: []
api_specs:
- filename: cybelangel-adm-inventory-api-openapi.yml
  format: yaml
  label: CybelAngel ADM Inventory API
  slug: cybelangel-adm-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-adm-inventory-api-openapi.yml
- filename: cybelangel-alerts-api-openapi.yml
  format: yaml
  label: CybelAngel Alerts API
  slug: cybelangel-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-alerts-api-openapi.yml
- filename: cybelangel-asset-api-openapi.yml
  format: yaml
  label: CybelAngel Asset API
  slug: cybelangel-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-asset-api-openapi.yml
- filename: cybelangel-audit-logs-api-openapi.yml
  format: yaml
  label: CybelAngel audit logs API
  slug: cybelangel-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-audit-logs-api-openapi.yml
- filename: cybelangel-credential-watchlist-api-openapi.yml
  format: yaml
  label: CybelAngel Credential watchlist API
  slug: cybelangel-credential-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-credential-watchlist-api-openapi.yml
- filename: cybelangel-domain-watchlist-api-openapi.yml
  format: yaml
  label: CybelAngel Domain watchlist API
  slug: cybelangel-domain-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-domain-watchlist-api-openapi.yml
- filename: cybelangel-incident-reports-api-openapi.yml
  format: yaml
  label: CybelAngel Incident reports API
  slug: cybelangel-incident-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-incident-reports-api-openapi.yml
- filename: cybelangel-keywords-api-openapi.yml
  format: yaml
  label: CybelAngel Keywords API
  slug: cybelangel-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-keywords-api-openapi.yml
- filename: cybelangel-reports-api-openapi.yml
  format: yaml
  label: CybelAngel Reports API
  slug: cybelangel-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-reports-api-openapi.yml
- filename: cybelangel-stats-api-openapi.yml
  format: yaml
  label: CybelAngel Stats API
  slug: cybelangel-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-stats-api-openapi.yml
- filename: cybelangel-stix-api-openapi.yml
  format: yaml
  label: CybelAngel Stix API
  slug: cybelangel-stix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-stix-api-openapi.yml
- filename: cybelangel-threat-intelligence-api-openapi.yml
  format: yaml
  label: CybelAngel Threat Intelligence API
  slug: cybelangel-threat-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-threat-intelligence-api-openapi.yml
- filename: cybelangel-workspaces-api-openapi.yml
  format: yaml
  label: CybelAngel Workspaces API
  slug: cybelangel-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-workspaces-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cybelangel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CybelAngel secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CybelAngel
provider_slug: cybelangel
scheme_count: 2
schemes:
- applied: root-level security requirement — every operation
  flows:
  - flow: clientCredentials
    scopes: 10
    tokenUrl: https://auth.cybelangel.com/oauth/token
  name: bearer_token
  see: scopes/cybelangel-scopes.yml
  sources:
  - openapi/cybelangel-platform-reports-openapi.yml
  type: oauth2
- applied: declared in components.securitySchemes; no root-level security requirement in these six specs
  bearerFormat: JWT
  gap: None of these six specs declares a root-level `security:` requirement or applies the scheme per operation, so a code generator reading them alone produces an unauthenticated client even though every endpoint returns 401 without a bearer. They also omit the token endpoint and any scope names.
  name: jwt
  scheme: bearer
  scopes: 0
  sources:
  - openapi/cybelangel-adm-inventory-openapi.yml
  - openapi/cybelangel-alerts-openapi.yml
  - openapi/cybelangel-audit-logs-openapi.yml
  - openapi/cybelangel-keywords-openapi.yml
  - openapi/cybelangel-partner-openapi.yml
  - openapi/cybelangel-threat-intelligence-openapi.yml
  type: http
slug: cybelangel-authentication
source_filename: cybelangel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: >-\n  openapi/cybelangel-adm-inventory-openapi.yml, openapi/cybelangel-alerts-openapi.yml,\n  openapi/cybelangel-audit-logs-openapi.yml, openapi/cybelangel-keywords-openapi.yml,\n  openapi/cybelangel-partner-openapi.yml, openapi/cybelangel-platform-reports-openapi.yml,\n  openapi/cybelangel-threat-intelligence-openapi.yml\ndocs:\n  - https://developers.cybelangel.com/docs/cybelangel-platform-api/b6b6c2d4906e9-authentication\n  - https://developers.cybelangel.com/docs/cybelangel-platform-api/05d245301ecc5-get-your-api-credentials\n  - https://developers.cybelangel.com/docs/cybelangel-platform-api/8ba3b4bfd2344-make-authenticated-requests\n  - https://developers.cybelangel.com/docs/audit-logs-api/b87d37ae48a0d-authentication\n  - https://developers.cybelangel.com/docs/alerts-api/fbe89213b575d-api-calls\nprobed:\n  - {url: 'https://auth.cybelangel.com/.well-known/openid-configuration', status: 200, file: well-known/cybelangel-openid-configuration.json}\n\
  \  - {url: 'https://auth.cybelangel.com/.well-known/oauth-authorization-server', status: 200, file: well-known/cybelangel-oauth-authorization-server.json}\n  - {url: 'https://auth.cybelangel.com/.well-known/jwks.json', status: 200, file: well-known/cybelangel-jwks.json}\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  single_credential: true\n  note: >-\n    One credential pair covers all seven APIs. The specs declare the mechanism inconsistently\n    but describe the same thing: the Reports API declares a full oauth2 clientCredentials\n    scheme with a tokenUrl and 10 named scopes, while the six api.cybelangel.com specs declare\n    only a bare `jwt` http-bearer scheme with no token endpoint and no scopes. The bearer they\n    accept is the same Auth0-issued token, so the http-bearer declarations are an\n    under-specification of the oauth2 flow rather than a second auth model. This artifact is\n    marked `searched` because the token endpoint,\
  \ audience, credential provisioning and quota\n    come from the docs, not from those six specs.\nauthorization_server:\n  issuer: https://auth.cybelangel.com/\n  vendor: Auth0\n  token_endpoint: https://auth.cybelangel.com/oauth/token\n  authorization_endpoint: https://auth.cybelangel.com/authorize\n  jwks_uri: https://auth.cybelangel.com/.well-known/jwks.json\n  revocation_endpoint: https://auth.cybelangel.com/oauth/revoke\n  userinfo_endpoint: https://auth.cybelangel.com/userinfo\n  registration_endpoint: https://auth.cybelangel.com/oidc/register\n  grant_types_supported: [client_credentials, authorization_code, refresh_token, password, implicit, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:ietf:params:oauth:grant-type:token-exchange', 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  code_challenge_methods_supported:\
  \ [S256, plain]\n  dpop_supported: true\n  note: >-\n    Most of the advertised grants belong to the platform's interactive login, not to the API.\n    The only grant the API documentation uses is client_credentials.\ntoken_request:\n  method: POST\n  url: https://auth.cybelangel.com/oauth/token\n  content_type: application/json\n  body_fields:\n    client_id: 'public identifier for your application'\n    client_secret: 'private secret used to generate tokens'\n    audience: 'https://platform.cybelangel.com/  — the same value for EVERY API, including api.cybelangel.com'\n    grant_type: client_credentials\n  response_fields: [access_token, scope, expires_in, token_type]\n  token_format: RS256 JWT\n  usage: 'Authorization: Bearer <access_token>'\n  note: >-\n    JSON body, not form-encoded — unusual for an OAuth token endpoint, and the shape the docs\n    publish in every curl example.\ncredential_provisioning:\n  location: 'CybelAngel Platform > Settings > CybelAngel API'\n  role_required:\
  \ 'CybelAngel Platform admin'\n  self_serve: true\n  actions: ['Enable API access (plan includes the API)', 'Start 30-day trial (plan does not)']\n  values_issued: [organization_id, client_id, client_secret]\n  organization_id_note: >-\n    Required in the path of the Audit Logs and Partner APIs, and NOT self-serve — the provider's\n    guide says \"To retrieve your organization ID, please contact your Customer Success Manager.\"\n  alerts_stream_id_note: >-\n    The Alerts API additionally requires a stream_id, also issued by a CSM (or via\n    support@cybelangel.com). Not obtainable from any API.\n  rotation: 'not documented — no key-rotation endpoint or policy published'\ntoken_lifetime:\n  assume_seconds: 3600\n  conflict: >-\n    The docs contradict themselves: 1 hour on the Reports and Audit Logs authentication pages,\n    24 hours on the Alerts \"API calls\" page, and expires_in 86400 in the Reports OpenAPI\n    description. Assume 3600 and refresh on 401.\n  sliding: 'the Alerts\
  \ limitations page says validity \"is renewed whenever it is used in a successfully authenticated request\"'\n  minting_quota: '2000 tokens/month per client_id — caching is mandatory, not optional'\nschemes:\n  - name: bearer_token\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.cybelangel.com/oauth/token\n        scopes: 10\n    applied: 'root-level security requirement — every operation'\n    sources:\n      - openapi/cybelangel-platform-reports-openapi.yml\n    see: scopes/cybelangel-scopes.yml\n  - name: jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applied: 'declared in components.securitySchemes; no root-level security requirement in these six specs'\n    scopes: 0\n    sources:\n      - openapi/cybelangel-adm-inventory-openapi.yml\n      - openapi/cybelangel-alerts-openapi.yml\n      - openapi/cybelangel-audit-logs-openapi.yml\n      - openapi/cybelangel-keywords-openapi.yml\n      - openapi/cybelangel-partner-openapi.yml\n\
  \      - openapi/cybelangel-threat-intelligence-openapi.yml\n    gap: >-\n      None of these six specs declares a root-level `security:` requirement or applies the scheme\n      per operation, so a code generator reading them alone produces an unauthenticated client\n      even though every endpoint returns 401 without a bearer. They also omit the token endpoint\n      and any scope names.\nerrors:\n  401: 'Missing or invalid token — verify the Authorization header format and regenerate a token'\n  403: 'Valid token, insufficient rights/scope — check that your API plan includes the required scope'\n  source: https://developers.cybelangel.com/docs/audit-logs-api/b87d37ae48a0d-authentication\nmtls: false\nopenid_connect_for_api: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/authentication/cybelangel-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Cybersecurity
- Threat Intelligence
- external-attack-surface-management
- data-breach-prevention
- Credential Intelligence
- Brand Protection
- Dark Web Monitoring
- Digital Risk Protection
- STIX
- security-alerts
- Asset Inventory
- Audit Logs
---
