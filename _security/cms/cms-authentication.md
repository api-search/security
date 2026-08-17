---
api_key_in:
- header
- query
api_specs:
- filename: cms-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: cms-beneficiary-claims-data-api-bcda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bcda-openapi.yml
- filename: cms-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API (Claims Data to Part D Sponsors)
  slug: cms-ab2d-api-claims-data-to-part-d-sponsors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-ab2d-openapi.yml
- filename: cms-api-reference-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services API Reference API
  slug: cms-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-api-reference-api-openapi.yml
- filename: cms-bulk-data-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Bulk Data API
  slug: cms-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bulk-data-api-openapi.yml
- filename: cms-code-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Code Search API
  slug: cms-code-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-code-search-api-openapi.yml
- filename: cms-cost-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Cost Search API
  slug: cms-cost-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-cost-search-api-openapi.yml
- filename: cms-enrollments-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Enrollments API
  slug: cms-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-enrollments-api-openapi.yml
- filename: cms-geography-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Geography API
  slug: cms-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-geography-api-openapi.yml
- filename: cms-households-eligibility-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Households & Eligibility API
  slug: cms-households-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-households-eligibility-api-openapi.yml
- filename: cms-insurance-issuers-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Issuers API
  slug: cms-insurance-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-issuers-api-openapi.yml
- filename: cms-insurance-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Plans API
  slug: cms-insurance-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-plans-api-openapi.yml
- filename: cms-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Plans API
  slug: cms-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-plans-api-openapi.yml
- filename: cms-provider-drug-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Provider & Drug Coverage API
  slug: cms-provider-drug-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-provider-drug-coverage-api-openapi.yml
- filename: cms-capability-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Capability API
  slug: centers-for-medicare-and-medicaid-services-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-capability-api-openapi.yml
- filename: cms-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Coverage API
  slug: centers-for-medicare-and-medicaid-services-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-coverage-api-openapi.yml
- filename: cms-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services ExplanationOfBenefit API
  slug: centers-for-medicare-and-medicaid-services-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-explanationofbenefit-api-openapi.yml
- filename: cms-patient-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Patient API
  slug: centers-for-medicare-and-medicaid-services-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-patient-api-openapi.yml
auth_types:
- apiKey
- http (bearer)
- http (basic)
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centers for Medicare and Medicaid Services secures its APIs with apiKey, http (bearer), http (basic), and oauth2 across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Centers for Medicare and Medicaid Services
provider_slug: cms
scheme_count: 9
schemes:
- api: CMS Blue Button 2.0 API
  authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize
  client_type: confidential
  description: Beneficiary-consent OAuth. The Medicare enrollee authenticates at Medicare.gov and grants the application access to their own claims data; the enrollee can revoke at any time.
  flow: authorizationCode
  guidance: For native and mobile apps CMS requires a Backend-For-Frontend proxy so all code and refresh exchanges happen server-side.
  name: Blue Button OAuth 2.0
  pkce: required (S256)
  revocationUrl: https://api.bluebutton.cms.gov/v2/o/revoke_token
  scopes: scopes/cms-scopes.yml
  sources:
  - https://bluebutton.cms.gov/api-documentation/authorization/
  - https://api.bluebutton.cms.gov/.well-known/openid-configuration
  tokenUrl: https://api.bluebutton.cms.gov/v2/o/token
  token_lifetime: access token 1 hour; refresh token supported
  type: oauth2
  unsupported:
  - implicit grant
  - public client type
  userinfoUrl: https://api.bluebutton.cms.gov/v2/connect/userinfo
- api: CMS Beneficiary Claims Data API (BCDA)
  description: BCDA's System-to-System Authentication Service (SSAS) issues a bearer token to an eligible model entity's registered client credentials. Credentials are managed in 4i and ACO-MS.
  in: header
  name: bearer_token
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/cms-bcda-openapi.yml
  - https://bcda.cms.gov/api-documentation/get-a-bearer-token.html
  token_endpoint: POST /auth/token
  token_endpoint_auth: HTTP Basic (client id + secret)
  type: http
- api: CMS Beneficiary Claims Data API (BCDA)
  description: Used only to authenticate the POST /auth/token exchange, not the data endpoints.
  name: basic_auth
  scheme: basic
  sources:
  - openapi/cms-bcda-openapi.yml
  type: http
- api: CMS AB2D API (Claims Data to Part D Sponsors)
  bearerFormat: JWT
  idp:
    production: idm.cms.gov
    sandbox: test.idp.idm.cms.gov
    vendor: Okta
  in: header
  name: bearerAuth
  network_control: Production additionally requires each calling system's static source IP address to be registered with CMS. This is why an anonymous probe of api.ab2d.cms.gov times out rather than returning 401.
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/cms-ab2d-openapi.yml
  - https://ab2d.cms.gov/api-documentation
  token_lifetime: 30 minutes
  type: http
- api: CMS Data at the Point of Care (DPC) API
  description: Declared in the DPC CapabilityStatement via the SMART oauth-uris extension and the restful-security-service code SMART-on-FHIR, text "SMART on FHIR Backend Services". Provider organizations register a public key and sign a JWT assertion to obtain a token.
  flow: clientCredentials (JWT client assertion)
  name: SMART on FHIR Backend Services
  sources:
  - conformance/cms-dpc-capabilitystatement.json
  - https://dpc.cms.gov/docsV1
  tokenUrl: https://dpc.cms.gov/api/v1/Token/auth
  type: oauth2
- api: Healthcare.gov Marketplace API
  caution: The key travels in the query string, so it lands in proxy and server access logs. There is no header alternative documented for this API.
  description: Your API key should be included as a query parameter with the request. Request one at https://developer.cms.gov/marketplace-api/key-request.html.
  in: query
  lifetime: 60 days, auto-renewed by email notification
  name: API Key
  parameter: apikey
  sources:
  - openapi/marketplace-openapi.json
  - https://developer.cms.gov/marketplace-api/key-request.html
  type: apiKey
- api: CMS Procedure Price Lookup (PPL) API
  description: All requests must include the `apiKey` header containing your API Key.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/ppl-openapi.json
  type: apiKey
- api: CMS Procedure Price Lookup (PPL) API
  description: All requests must include the `amaLicense` header containing your AMA License. This is a separately purchased annual American Medical Association CPT license — the only paid precondition anywhere in the CMS API surface. Missing or invalid returns HTTP 403.
  in: header
  name: amaLicense
  parameter: amaLicense
  sources:
  - openapi/ppl-openapi.json
  - https://developer.cms.gov/ppl-api/
  type: apiKey
- api: CMS Provider Data Catalog API / NPPES NPI Registry API
  description: 'Fully open. Probed anonymously on 2026-08-15: https://npiregistry.cms.hhs.gov/api/ returned 200 without any credential, and https://data.cms.gov/provider-data/api/1/metastore/schemas/dataset/items returned 200 with a 290 KB DCAT dataset collection.'
  name: none
  type: none
slug: cms-authentication
source_filename: cms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: >-\n  openapi/marketplace-openapi.json, openapi/ppl-openapi.json, openapi/cms-bcda-openapi.yml,\n  openapi/cms-ab2d-openapi.yml, openapi/_original/cms-cms-blue-button-2-openapi.yml\ndocs:\n  - https://bluebutton.cms.gov/api-documentation/authorization/\n  - https://bcda.cms.gov/api-documentation/get-a-bearer-token.html\n  - https://ab2d.cms.gov/get-a-bearer-token\n  - https://dpc.cms.gov/docsV1\n  - https://developer.cms.gov/marketplace-api/key-request.html\n  - https://developer.cms.gov/ppl-api/\ndiscovery: https://api.bluebutton.cms.gov/.well-known/openid-configuration\nupgrade_note: >-\n  Upgraded 2026-08-15 from derived to searched. The 2026-07-11 derived pass saw only the Marketplace\n  and PPL API-key schemes because those were the only harvested specs with securitySchemes. The BCDA\n  and AB2D OpenAPIs discovered in this pass add the bearer schemes, and the CMS authorization docs add\n  the Blue Button OAuth profile\
  \ and the DPC SMART Backend Services profile.\nsummary:\n  types:\n    - apiKey\n    - http (bearer)\n    - http (basic)\n    - oauth2\n  api_key_in:\n    - header\n    - query\n  note: >-\n    Five distinct authentication models across one agency. There is no single CMS credential and no\n    single CMS identity provider: BCDA issues its own tokens via SSAS, AB2D federates to Okta, Blue\n    Button runs its own OAuth server against Medicare.gov login, DPC uses SMART Backend Services JWT\n    assertions, and the Marketplace surface is plain API keys. A developer integrating two CMS APIs\n    implements two auth stacks.\nschemes:\n  - name: Blue Button OAuth 2.0\n    api: CMS Blue Button 2.0 API\n    type: oauth2\n    flow: authorizationCode\n    pkce: required (S256)\n    client_type: confidential\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token\n    revocationUrl: https://api.bluebutton.cms.gov/v2/o/revoke_token\n\
  \    userinfoUrl: https://api.bluebutton.cms.gov/v2/connect/userinfo\n    token_lifetime: access token 1 hour; refresh token supported\n    scopes: scopes/cms-scopes.yml\n    unsupported:\n      - implicit grant\n      - public client type\n    guidance: >-\n      For native and mobile apps CMS requires a Backend-For-Frontend proxy so all code and refresh\n      exchanges happen server-side.\n    description: >-\n      Beneficiary-consent OAuth. The Medicare enrollee authenticates at Medicare.gov and grants the\n      application access to their own claims data; the enrollee can revoke at any time.\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n      - https://api.bluebutton.cms.gov/.well-known/openid-configuration\n  - name: bearer_token\n    api: CMS Beneficiary Claims Data API (BCDA)\n    type: http\n    in: header\n    parameter: Authorization\n    scheme: bearer\n    token_endpoint: POST /auth/token\n    token_endpoint_auth: HTTP Basic (client\
  \ id + secret)\n    description: >-\n      BCDA's System-to-System Authentication Service (SSAS) issues a bearer token to an eligible model\n      entity's registered client credentials. Credentials are managed in 4i and ACO-MS.\n    sources:\n      - openapi/cms-bcda-openapi.yml\n      - https://bcda.cms.gov/api-documentation/get-a-bearer-token.html\n  - name: basic_auth\n    api: CMS Beneficiary Claims Data API (BCDA)\n    type: http\n    scheme: basic\n    description: Used only to authenticate the POST /auth/token exchange, not the data endpoints.\n    sources:\n      - openapi/cms-bcda-openapi.yml\n  - name: bearerAuth\n    api: CMS AB2D API (Claims Data to Part D Sponsors)\n    type: http\n    in: header\n    parameter: Authorization\n    scheme: bearer\n    bearerFormat: JWT\n    idp:\n      production: idm.cms.gov\n      sandbox: test.idp.idm.cms.gov\n      vendor: Okta\n    token_lifetime: 30 minutes\n    network_control: >-\n      Production additionally requires each calling\
  \ system's static source IP address to be registered\n      with CMS. This is why an anonymous probe of api.ab2d.cms.gov times out rather than returning 401.\n    sources:\n      - openapi/cms-ab2d-openapi.yml\n      - https://ab2d.cms.gov/api-documentation\n  - name: SMART on FHIR Backend Services\n    api: CMS Data at the Point of Care (DPC) API\n    type: oauth2\n    flow: clientCredentials (JWT client assertion)\n    tokenUrl: https://dpc.cms.gov/api/v1/Token/auth\n    description: >-\n      Declared in the DPC CapabilityStatement via the SMART oauth-uris extension and the\n      restful-security-service code SMART-on-FHIR, text \"SMART on FHIR Backend Services\". Provider\n      organizations register a public key and sign a JWT assertion to obtain a token.\n    sources:\n      - conformance/cms-dpc-capabilitystatement.json\n      - https://dpc.cms.gov/docsV1\n  - name: API Key\n    api: Healthcare.gov Marketplace API\n    type: apiKey\n    in: query\n    parameter: apikey\n    lifetime:\
  \ 60 days, auto-renewed by email notification\n    description: >-\n      Your API key should be included as a query parameter with the request. Request one at\n      https://developer.cms.gov/marketplace-api/key-request.html.\n    sources:\n      - openapi/marketplace-openapi.json\n      - https://developer.cms.gov/marketplace-api/key-request.html\n    caution: >-\n      The key travels in the query string, so it lands in proxy and server access logs. There is no\n      header alternative documented for this API.\n  - name: apiKey\n    api: CMS Procedure Price Lookup (PPL) API\n    type: apiKey\n    in: header\n    parameter: apiKey\n    description: All requests must include the `apiKey` header containing your API Key.\n    sources:\n      - openapi/ppl-openapi.json\n  - name: amaLicense\n    api: CMS Procedure Price Lookup (PPL) API\n    type: apiKey\n    in: header\n    parameter: amaLicense\n    description: >-\n      All requests must include the `amaLicense` header containing your\
  \ AMA License. This is a\n      separately purchased annual American Medical Association CPT license — the only paid\n      precondition anywhere in the CMS API surface. Missing or invalid returns HTTP 403.\n    sources:\n      - openapi/ppl-openapi.json\n      - https://developer.cms.gov/ppl-api/\n  - name: none\n    api: CMS Provider Data Catalog API / NPPES NPI Registry API\n    type: none\n    description: >-\n      Fully open. Probed anonymously on 2026-08-15: https://npiregistry.cms.hhs.gov/api/ returned 200\n      without any credential, and https://data.cms.gov/provider-data/api/1/metastore/schemas/dataset/items\n      returned 200 with a 290 KB DCAT dataset collection.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/authentication/cms-authentication.yml
summary_line: apiKey/http (bearer)/http (basic)/oauth2 · 9 schemes
tags:
- Medicare
- Medicaid
- Healthcare
- Health Insurance
- FHIR
- Federal Government
- Drug Spending
- Provider Data
- Quality Measures
- Claims Data
---
