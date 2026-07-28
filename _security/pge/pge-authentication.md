---
api_key_in: []
api_specs:
- filename: green-button-alliance-espi-openapi.json
  format: json
  label: PG&E Share My Data (Green Button Connect My Data) ESPI API
  slug: pge-share-my-data-espi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/green-button-alliance-espi-openapi.json
auth_types:
- oauth2
- mutualTLS
- http
description: 'PG&E Share My Data authenticates third parties with OAuth 2.0 (NAESB ESPI authorization profile) layered on MANDATORY mutual TLS 1.2. This is not OpenID Connect: /.well-known/openid-configuration returns HTTP 404 on www.pge.com, api.pge.com and sharemydata.pge.com (re-probed 2026-07-27). Two bearer-token classes are issued from separate grants, and a third registration token governs the ApplicationInformation resource.'
kind: authentication
layout: security
method: searched
name: Pge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Pacific Gas and Electric secures its APIs with oauth2, mutualTLS, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Pacific Gas and Electric
provider_slug: pge
scheme_count: 5
schemes:
- applies_to: Every request between the third party and PG&E except the browser redirects in the OAuth authorization-code flow, including the token endpoint call.
  certificate: Third party must present an unexpired, unrevoked SHA-2 X.509 client certificate with an RSA public key of at least 2048 bits, issued by a recognized public certificate authority. PG&E names AddTrust, Comodo, DigiCert, Entrust, GlobalSign, Go Daddy, USERTrust and VeriSign. Self-signed certificates are explicitly not accepted.
  name: MutualTLS
  required: true
  source: docs
  tls_version: TLS 1.2
  type: mutualTLS
  verified: Anonymous GET of every ESPI resource path returns HTTP 400 "Invalid Certificate" from Mulesoft-API-Gateway, while invented sibling paths return HTTP 404 "No listener for endpoint" (2026-07-27).
- client_authentication: 'HTTP Basic — Authorization: Basic base64(client_ID:client_Secret) — with grant_type=client_credentials.'
  flow: clientCredentials
  issues: client_access_token
  name: OAuth2ClientCredentials
  refresh_token_lifetime: 1 year
  response_format: XML Response document with client_access_token, expires_in, scope and token_type elements (PG&E's published connectivity-test example).
  source: docs
  test_token_endpoint: https://api.pge.com/datacustodian/test/oauth/v2/token
  token_endpoint: https://api.pge.com/datacustodian/oauth/v2/token
  token_lifetime_seconds: 3600
  token_type: Bearer
  type: oauth2
  used_for: Third-party-level resources — DownloadSampleData, ReadServiceStatus, the Authorization feed and detail, and the Bulk-level Batch resources.
- authorization_code_lifetime_seconds: 600
  authorization_endpoint_production: https://sharemydata.pge.com/myAuthorization
  authorization_endpoint_test: https://api.pge.com/datacustodian/test/oauth/v2/authorize
  client_authentication: 'HTTP Basic — Authorization: Basic base64(client_ID:client_Secret) — with grant_type=authorization_code, code and redirect_uri.'
  customer_journey: The PG&E customer authenticates on PG&E's own site (or the Guest Access tab) and selects data groups, interval duration and authorization period (defined period or Indefinite). A customer may cancel; a third party may revoke with HTTP DELETE on the Authorization resource.
  flow: authorizationCode
  issues: access_token + refresh_token
  name: OAuth2AuthorizationCode
  refresh_token_lifetime: 1 year
  scope_model: ESPI function-block scope string rather than named OAuth scopes — see scopes/pge-scopes.yml.
  source: docs
  state_parameter: supported (optional, echoed back)
  test_token_endpoint: https://api.pge.com/datacustodian/test/oauth/v2/token
  token_endpoint: https://api.pge.com/datacustodian/oauth/v2/token
  token_lifetime_seconds: 3600
  token_type: bearer
  type: oauth2
  used_for: Per-customer resources — LocalTimeParameters, ReadingType, the Subscription/UsagePoint/MeterReading/IntervalBlock/UsageSummary trees and the customer-level Batch resources.
- issued_at: registration, via the Share My Data third-party portal
  name: RegistrationAccessToken
  scheme: bearer
  source: docs
  token: registration_access_token
  type: http
  used_for: The ApplicationInformation resource, which returns the third party's own registered application record.
- first_party: false
  flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  note: Retained from the derived pass over the Green Button Alliance OpenAPI. Its URLs are the GBA sandbox (https://sandbox.greenbuttonalliance.org:8443), NOT PG&E hosts. Kept only to document the standard contract.
  sources:
  - openapi/green-button-alliance-espi-openapi.json
  type: oauth2
slug: pge-authentication
source_filename: pge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\n  (HTTP 200, fetched 2026-07-27) and\n  https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/OAuth_Authorization_ESPI.pdf\n  (HTTP 200). Upgraded from the derived pass over\n  openapi/green-button-alliance-espi-openapi.json, whose declared server is the\n  Green Button Alliance sandbox and NOT a PG&E host.\ndocs: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\ndescription: >-\n  PG&E Share My Data authenticates third parties with OAuth 2.0 (NAESB ESPI\n  authorization profile) layered on MANDATORY mutual TLS 1.2. This is not\n  OpenID Connect: /.well-known/openid-configuration returns HTTP 404 on\n  www.pge.com, api.pge.com and sharemydata.pge.com (re-probed 2026-07-27). Two\n  bearer-token classes are issued from separate grants,\
  \ and a third\n  registration token governs the ApplicationInformation resource.\nsummary:\n  types: [oauth2, mutualTLS, http]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in: []\n  openid_connect: false\n  mutual_tls_required: true\nschemes:\n  - name: MutualTLS\n    type: mutualTLS\n    required: true\n    tls_version: TLS 1.2\n    certificate: >-\n      Third party must present an unexpired, unrevoked SHA-2 X.509 client\n      certificate with an RSA public key of at least 2048 bits, issued by a\n      recognized public certificate authority. PG&E names AddTrust, Comodo,\n      DigiCert, Entrust, GlobalSign, Go Daddy, USERTrust and VeriSign.\n      Self-signed certificates are explicitly not accepted.\n    applies_to: >-\n      Every request between the third party and PG&E except the browser\n      redirects in the OAuth authorization-code flow, including the token\n      endpoint call.\n    verified: >-\n      Anonymous GET of every ESPI resource\
  \ path returns HTTP 400 \"Invalid\n      Certificate\" from Mulesoft-API-Gateway, while invented sibling paths\n      return HTTP 404 \"No listener for endpoint\" (2026-07-27).\n    source: docs\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://api.pge.com/datacustodian/oauth/v2/token\n    test_token_endpoint: https://api.pge.com/datacustodian/test/oauth/v2/token\n    client_authentication: >-\n      HTTP Basic — Authorization: Basic base64(client_ID:client_Secret) — with\n      grant_type=client_credentials.\n    issues: client_access_token\n    token_type: Bearer\n    token_lifetime_seconds: 3600\n    refresh_token_lifetime: 1 year\n    response_format: >-\n      XML Response document with client_access_token, expires_in, scope and\n      token_type elements (PG&E's published connectivity-test example).\n    used_for: >-\n      Third-party-level resources — DownloadSampleData, ReadServiceStatus, the\n      Authorization feed\
  \ and detail, and the Bulk-level Batch resources.\n    source: docs\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint_production: https://sharemydata.pge.com/myAuthorization\n    authorization_endpoint_test: https://api.pge.com/datacustodian/test/oauth/v2/authorize\n    token_endpoint: https://api.pge.com/datacustodian/oauth/v2/token\n    test_token_endpoint: https://api.pge.com/datacustodian/test/oauth/v2/token\n    client_authentication: >-\n      HTTP Basic — Authorization: Basic base64(client_ID:client_Secret) — with\n      grant_type=authorization_code, code and redirect_uri.\n    authorization_code_lifetime_seconds: 600\n    issues: access_token + refresh_token\n    token_type: bearer\n    token_lifetime_seconds: 3600\n    refresh_token_lifetime: 1 year\n    state_parameter: supported (optional, echoed back)\n    scope_model: >-\n      ESPI function-block scope string rather than named OAuth scopes — see\n      scopes/pge-scopes.yml.\n\
  \    used_for: >-\n      Per-customer resources — LocalTimeParameters, ReadingType, the\n      Subscription/UsagePoint/MeterReading/IntervalBlock/UsageSummary trees and\n      the customer-level Batch resources.\n    customer_journey: >-\n      The PG&E customer authenticates on PG&E's own site (or the Guest Access\n      tab) and selects data groups, interval duration and authorization period\n      (defined period or Indefinite). A customer may cancel; a third party may\n      revoke with HTTP DELETE on the Authorization resource.\n    source: docs\n  - name: RegistrationAccessToken\n    type: http\n    scheme: bearer\n    token: registration_access_token\n    issued_at: registration, via the Share My Data third-party portal\n    used_for: >-\n      The ApplicationInformation resource, which returns the third party's own\n      registered application record.\n    source: docs\n  - name: oauth2\n    type: oauth2\n    first_party: false\n    note: >-\n      Retained from the derived pass\
  \ over the Green Button Alliance OpenAPI. Its\n      URLs are the GBA sandbox (https://sandbox.greenbuttonalliance.org:8443),\n      NOT PG&E hosts. Kept only to document the standard contract.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n        tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n        scopes: 0\n      - flow: clientCredentials\n        tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n        scopes: 0\n    sources:\n      - openapi/green-button-alliance-espi-openapi.json\nopenid_connect:\n  served: false\n  probed: '2026-07-27'\n  probes:\n    - {url: 'https://www.pge.com/.well-known/openid-configuration', status: 404}\n    - {url: 'https://api.pge.com/.well-known/openid-configuration', status: 404}\n    - {url: 'https://sharemydata.pge.com/.well-known/openid-configuration', status: 404}\noauth_metadata:\n  rfc8414_served: false\n  probed: '2026-07-27'\n\
  \  probes:\n    - {url: 'https://api.pge.com/.well-known/oauth-authorization-server', status: 404}\n    - {url: 'https://www.pge.com/.well-known/oauth-authorization-server', status: 404}\naccess_gate: >-\n  Credentials are not self-serve. A client_id/client_secret pair is issued only\n  after registration at https://sharemydata.pge.com/ with a US EIN, CPUC\n  eligibility screening, tariff acceptance and completion of the mandatory\n  connectivity and OAuth tests within 90 days.\nrelated:\n  - scopes/pge-scopes.yml\n  - conventions/pge-conventions.yml\n  - sandbox/pge-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/authentication/pge-authentication.yml
summary_line: oauth2/mutualTLS/http · 5 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- California
- Smart Metering
- Green Button
- ESPI
- Energy Data
- Grid
- Demand Response
- Investor-Owned Utility
---
