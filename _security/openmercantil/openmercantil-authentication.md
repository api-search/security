---
api_key_in:
- cookie
- header
api_specs:
- filename: openmercantil-api-credentials-api-openapi.yml
  format: yaml
  label: OpenMercantil API Credentials API
  slug: openmercantil-api-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-api-credentials-api-openapi.yml
- filename: openmercantil-billing-api-openapi.yml
  format: yaml
  label: OpenMercantil Billing API
  slug: openmercantil-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-billing-api-openapi.yml
- filename: openmercantil-borme-api-openapi.yml
  format: yaml
  label: OpenMercantil BORME API
  slug: openmercantil-borme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-borme-api-openapi.yml
- filename: openmercantil-companies-api-openapi.yml
  format: yaml
  label: OpenMercantil Companies API
  slug: openmercantil-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-companies-api-openapi.yml
- filename: openmercantil-datasets-api-openapi.yml
  format: yaml
  label: OpenMercantil Datasets API
  slug: openmercantil-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-datasets-api-openapi.yml
- filename: openmercantil-graph-api-openapi.yml
  format: yaml
  label: OpenMercantil Graph API
  slug: openmercantil-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-graph-api-openapi.yml
- filename: openmercantil-integrations-api-openapi.yml
  format: yaml
  label: OpenMercantil Integrations API
  slug: openmercantil-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-integrations-api-openapi.yml
- filename: openmercantil-legal-api-openapi.yml
  format: yaml
  label: OpenMercantil Legal API
  slug: openmercantil-legal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-legal-api-openapi.yml
- filename: openmercantil-persons-api-openapi.yml
  format: yaml
  label: OpenMercantil Persons API
  slug: openmercantil-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-persons-api-openapi.yml
- filename: openmercantil-public-procurement-api-openapi.yml
  format: yaml
  label: OpenMercantil Public Procurement API
  slug: openmercantil-public-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-public-procurement-api-openapi.yml
- filename: openmercantil-risk-signals-api-openapi.yml
  format: yaml
  label: OpenMercantil Risk Signals API
  slug: openmercantil-risk-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-risk-signals-api-openapi.yml
- filename: openmercantil-search-api-openapi.yml
  format: yaml
  label: OpenMercantil Search API
  slug: openmercantil-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-search-api-openapi.yml
- filename: openmercantil-sectors-api-openapi.yml
  format: yaml
  label: OpenMercantil Sectors API
  slug: openmercantil-sectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sectors-api-openapi.yml
- filename: openmercantil-sources-api-openapi.yml
  format: yaml
  label: OpenMercantil Sources API
  slug: openmercantil-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sources-api-openapi.yml
- filename: openmercantil-support-api-openapi.yml
  format: yaml
  label: OpenMercantil Support API
  slug: openmercantil-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-support-api-openapi.yml
- filename: openmercantil-system-api-openapi.yml
  format: yaml
  label: OpenMercantil System API
  slug: openmercantil-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-system-api-openapi.yml
- filename: openmercantil-user-api-openapi.yml
  format: yaml
  label: OpenMercantil User API
  slug: openmercantil-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-user-api-openapi.yml
- filename: openmercantil-webhooks-api-openapi.yml
  format: yaml
  label: OpenMercantil Webhooks API
  slug: openmercantil-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: 'Authentication profile for the OpenMercantil v1 REST API. The public read plane is ANONYMOUS BY DEFAULT — the documentation states plainly "REST + JSON. Sin autenticacion. CORS abierto." and every quickstart example is an unauthenticated curl. A credential is therefore optional on public reads and serves to select the account quota rather than to grant access. Three schemes are declared: an optional opaque omk_* API credential presented as X-API-Key or as Authorization: Bearer, and a browser session cookie for the account plane. There is no OAuth 2.0, no OIDC and no JWT anywhere in the contract.'
kind: authentication
layout: security
method: searched
name: Openmercantil Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMercantil secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenMercantil
provider_slug: openmercantil
scheme_count: 3
schemes:
- description: Browser session cookie set after login at /mi-cuenta/login. Mutations also require X-CSRF-Token header (obtain via GET /api/v1/user/me).
  in: cookie
  name: cookieAuth
  parameter: ob_sess
  sources:
  - openapi/openmercantil-api-credentials-api-openapi.yml
  - openapi/openmercantil-billing-api-openapi.yml
  - openapi/openmercantil-companies-api-openapi.yml
  - openapi/openmercantil-legal-api-openapi.yml
  - openapi/openmercantil-support-api-openapi.yml
  - openapi/openmercantil-user-api-openapi.yml
  - openapi/openmercantil-webhooks-api-openapi.yml
  type: apiKey
- description: Optional opaque omk_* API credential for public GETs. Anonymous access remains valid; a credential with the operation's x-api-credential-scope (or public:read) selects its account quota. Never place credentials in query strings.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/openmercantil-borme-api-openapi.yml
  - openapi/openmercantil-companies-api-openapi.yml
  - openapi/openmercantil-datasets-api-openapi.yml
  - openapi/openmercantil-graph-api-openapi.yml
  - openapi/openmercantil-integrations-api-openapi.yml
  - openapi/openmercantil-legal-api-openapi.yml
  - openapi/openmercantil-persons-api-openapi.yml
  - openapi/openmercantil-public-procurement-api-openapi.yml
  - openapi/openmercantil-search-api-openapi.yml
  - openapi/openmercantil-sectors-api-openapi.yml
  - openapi/openmercantil-sources-api-openapi.yml
  - openapi/openmercantil-system-api-openapi.yml
  type: apiKey
- bearerFormat: opaque omk_* credential
  description: 'Optional Authorization: Bearer transport for the same opaque omk_* API credential accepted by X-API-Key. It is not a JWT or OAuth access token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openmercantil-borme-api-openapi.yml
  - openapi/openmercantil-companies-api-openapi.yml
  - openapi/openmercantil-datasets-api-openapi.yml
  - openapi/openmercantil-graph-api-openapi.yml
  - openapi/openmercantil-integrations-api-openapi.yml
  - openapi/openmercantil-legal-api-openapi.yml
  - openapi/openmercantil-persons-api-openapi.yml
  - openapi/openmercantil-public-procurement-api-openapi.yml
  - openapi/openmercantil-search-api-openapi.yml
  - openapi/openmercantil-sectors-api-openapi.yml
  - openapi/openmercantil-sources-api-openapi.yml
  - openapi/openmercantil-system-api-openapi.yml
  type: http
slug: openmercantil-authentication
source_filename: openmercantil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://openmercantil.es/api/documentacion and openapi/_original/openmercantil-openapi-1.9.3.json\ndocs: https://openmercantil.es/api/documentacion\ndescription: 'Authentication profile for the OpenMercantil v1 REST API. The public read plane is ANONYMOUS\n  BY DEFAULT — the documentation states plainly \"REST + JSON. Sin autenticacion. CORS abierto.\" and every\n  quickstart example is an unauthenticated curl. A credential is therefore optional on public reads and\n  serves to select the account quota rather than to grant access. Three schemes are declared: an optional\n  opaque omk_* API credential presented as X-API-Key or as Authorization: Bearer, and a browser session\n  cookie for the account plane. There is no OAuth 2.0, no OIDC and no JWT anywhere in the contract.'\nmodel: optional-api-key-plus-session-cookie\nanonymous_access: true\noauth2: false\noidc: false\njwt: false\nmutual_tls: false\nsummary:\n  types:\n  -\
  \ apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: ob_sess\n  description: Browser session cookie set after login at /mi-cuenta/login. Mutations also require X-CSRF-Token\n    header (obtain via GET /api/v1/user/me).\n  sources:\n  - openapi/openmercantil-api-credentials-api-openapi.yml\n  - openapi/openmercantil-billing-api-openapi.yml\n  - openapi/openmercantil-companies-api-openapi.yml\n  - openapi/openmercantil-legal-api-openapi.yml\n  - openapi/openmercantil-support-api-openapi.yml\n  - openapi/openmercantil-user-api-openapi.yml\n  - openapi/openmercantil-webhooks-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional opaque omk_* API credential for public GETs. Anonymous access remains valid; a\n    credential with the operation's x-api-credential-scope (or public:read) selects its account quota.\n    Never place credentials in query strings.\n\
  \  sources:\n  - openapi/openmercantil-borme-api-openapi.yml\n  - openapi/openmercantil-companies-api-openapi.yml\n  - openapi/openmercantil-datasets-api-openapi.yml\n  - openapi/openmercantil-graph-api-openapi.yml\n  - openapi/openmercantil-integrations-api-openapi.yml\n  - openapi/openmercantil-legal-api-openapi.yml\n  - openapi/openmercantil-persons-api-openapi.yml\n  - openapi/openmercantil-public-procurement-api-openapi.yml\n  - openapi/openmercantil-search-api-openapi.yml\n  - openapi/openmercantil-sectors-api-openapi.yml\n  - openapi/openmercantil-sources-api-openapi.yml\n  - openapi/openmercantil-system-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque omk_* credential\n  description: 'Optional Authorization: Bearer transport for the same opaque omk_* API credential accepted\n    by X-API-Key. It is not a JWT or OAuth access token.'\n  sources:\n  - openapi/openmercantil-borme-api-openapi.yml\n  - openapi/openmercantil-companies-api-openapi.yml\n\
  \  - openapi/openmercantil-datasets-api-openapi.yml\n  - openapi/openmercantil-graph-api-openapi.yml\n  - openapi/openmercantil-integrations-api-openapi.yml\n  - openapi/openmercantil-legal-api-openapi.yml\n  - openapi/openmercantil-persons-api-openapi.yml\n  - openapi/openmercantil-public-procurement-api-openapi.yml\n  - openapi/openmercantil-search-api-openapi.yml\n  - openapi/openmercantil-sectors-api-openapi.yml\n  - openapi/openmercantil-sources-api-openapi.yml\n  - openapi/openmercantil-system-api-openapi.yml\nplanes:\n- name: public read plane\n  auth: none required; optional omk_* credential for account quota\n  schemes:\n  - apiKey\n  - bearerAuth\n  operations: 43\n  note: 43 operations declare an x-api-credential-scope; the rest of the public plane accepts the public:read\n    umbrella scope.\n- name: account plane\n  auth: ob_sess session cookie + X-CSRF-Token on mutations\n  schemes:\n  - cookieAuth\n  operations: 65\n  note: API credentials are NOT accepted here. Missing\
  \ or stale CSRF is the dominant 403 in the contract.\n- name: provider callback\n  auth: Stripe signature over raw request bytes\n  schemes: []\n  operations: 1\n  operation: receiveStripeWebhook\ncredential:\n  prefix: omk_\n  opaque: true\n  jwt: false\n  transports:\n  - X-API-Key header\n  - 'Authorization: Bearer header'\n  query_string_permitted: false\n  issued_at: https://openmercantil.es/mi-cuenta\n  management_operations:\n  - listUserApiCredentials\n  - createUserApiCredential\n  - rotateUserApiCredential\n  - revokeUserApiCredential\n  secret_visibility: returned once; recoverable only via an identical Idempotency-Key replay inside 24\n    hours\n  scopes: scopes/openmercantil-scopes.yml\ncsrf:\n  required_on: all account-plane mutations\n  header: X-CSRF-Token\n  obtain_via: GET /api/v1/user/me\nhuman_login:\n  methods:\n  - email + password\n  - Google Sign-In\n  url: https://openmercantil.es/mi-cuenta/login\n  password_hashing: bcrypt cost 12\n  breach_check: HaveIBeenPwned\
  \ on password change\n  note: Web login only. Google Sign-In is not an API authorization surface — there is no OIDC discovery\n    document.\ndiscovery_probes:\n- url: https://openmercantil.es/.well-known/openid-configuration\n  status: 404\n- url: https://openmercantil.es/.well-known/oauth-authorization-server\n  status: 404\n- url: https://openmercantil.es/.well-known/oauth-protected-resource\n  status: 404\n- url: https://openmercantil.es/api/v1/user/me\n  status: 401\n  note: correctly 401s when unauthenticated\nsee_also:\n  scopes: scopes/openmercantil-scopes.yml\n  conventions: conventions/openmercantil-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/authentication/openmercantil-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- BDNS
- BORME
- Business Registry
- CIF
- CNAE
- CNMV
- CSV
- Company Data
- Company Search
- Corporate Registry
- DCAT-AP
- Daily Summary
- Geocoding
- JSON
- Legal Data
- Mercantile Law
- OEPM
- Open Data
- Open Government Data
- OpenAPI
- OpenSanctions
- PLACSP
- Public Procurement
- Public Records
- Public-Interest Data
- REST API
- Registry Timeline
- Risk Signals
- Sanctions
- Spain
- Spanish Companies
- Spanish Open Data
- Tenders
- Trust Score
- Webhook
---
