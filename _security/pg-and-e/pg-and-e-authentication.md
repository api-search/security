---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pg-and-e-authorization-api-openapi.yml
  format: yaml
  label: pg-and-e Authorization API
  slug: pg-and-e-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-authorization-api-openapi.yml
- filename: pg-and-e-subscriptions-api-openapi.yml
  format: yaml
  label: pg-and-e Subscriptions API
  slug: pg-and-e-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-subscriptions-api-openapi.yml
- filename: pg-and-e-usage-api-openapi.yml
  format: yaml
  label: pg-and-e Usage API
  slug: pg-and-e-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-usage-api-openapi.yml
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pg And E Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- refresh_token
overview: Pg And E secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, and refresh_token flow(s).
provider_name: Pg And E
provider_slug: pg-and-e
scheme_count: 2
schemes:
- evidence:
  - body: '"Invalid Certificate"'
    fetched: '2026-09-17'
    status: 400
    url: https://api.pge.com/GreenButtonConnect/espi/1_1/resource/Authorization
  - body: '"Invalid Certificate"'
    fetched: '2026-09-17'
    status: 400
    url: https://api.pge.com/GreenButtonConnect/espi/1_1/resource/ReadServiceStatus
  name: mutual_tls
  required: true
  requirement: A valid TLS 1.2 X.509 certificate issued by a recognized SSL provider. PG&E states "Self-signed certificates are not accepted and submission of a self-signed SSL certificate will delay the approval of your registration."
  scope: every call to api.pge.com, including the OAuth token endpoint
  source: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html
  type: mutualTLS
- evidence:
  - body: '{"error":"invalid_request","error_description":"GET not permitted"}'
    fetched: '2026-09-17'
    method: GET
    status: 405
    url: https://api.pge.com/datacustodian/oauth/v2/token
  - body: '{"error":"invalid_request","error_description":"Missing grant_type"}'
    fetched: '2026-09-17'
    method: GET
    status: 400
    url: https://api.pge.com/datacustodian/test/oauth/v2/token
  - body: '{"error":"invalid_request","error_description":"client_id is empty"}'
    fetched: '2026-09-17'
    method: GET
    status: 400
    url: https://api.pge.com/datacustodian/test/oauth/v2/authorize
  flows:
  - description: Third-party-level token. Used for the third party's own resources — ApplicationInformation, the Authorization feed, ReadServiceStatus, and every Bulk resource (Batch/Bulk/{BulkID}, Batch/BulkRetailCustomerInfo/{BulkID}, Batch/BulkRetailDRPrgInfo/{BulkID}).
    flow: client_credentials
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
    token_class: client_access_token
  - authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/Authorize
    description: Per-customer token, issued after a PG&E customer authenticates on PG&E's own site and chooses what to share. Used for every customer-scoped resource under Subscription/{SubscriptionID}/... . Paired with a refresh token.
    flow: authorization_code
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
    token_class: access_token
  - description: Refreshes the per-customer access token.
    flow: refresh_token
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  name: oauth2
  revocation:
    description: Cancels an individual customer authorization.
    operation: DELETE /GreenButtonConnect/espi/1_1/resource/Authorization/{AuthorizationID}
    token: client_access_token
  scope_format: ESPI function-block string — see scopes/pg-and-e-scopes.yml
  sources:
  - https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/OAuth_Authorization_ESPI.pdf
  - https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-APIs.pdf
  type: oauth2
slug: pg-and-e-authentication
source_filename: pg-and-e-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: pg-and-e\nproviderId: pg-and-e\ngenerated: '2026-09-17'\nmethod: searched\nsource: https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/OAuth_Authorization_ESPI.pdf\ndocs: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\nmodified: '2026-09-17'\nnote: >-\n  Supersedes the 2026-07-11 derived artifact, which read a single authorizationCode flow out of the\n  in-repo OpenAPI scaffold and missed the two facts that actually decide whether an agent can call\n  this API: there are TWO token classes, and every call runs over MANDATORY mutual TLS with a\n  CA-issued client certificate. Both are published anonymously by PG&E and both were confirmed live\n  on 2026-09-17.\nsummary:\n  types:\n    - oauth2\n    - mutualTLS\n  oauth2_flows:\n    - authorization_code\n    - client_credentials\n    - refresh_token\n  transport_auth:\
  \ mutual TLS 1.2 (client X.509 certificate)\n  openid_connect: false\n  openid_connect_evidence: >-\n    /.well-known/openid-configuration returns HTTP 404 on www.pge.com, api.pge.com and\n    sharemydata.pge.com (probed 2026-09-17). This is plain OAuth 2.0, not OpenID Connect.\nschemes:\n  - name: mutual_tls\n    type: mutualTLS\n    required: true\n    scope: every call to api.pge.com, including the OAuth token endpoint\n    requirement: >-\n      A valid TLS 1.2 X.509 certificate issued by a recognized SSL provider. PG&E states\n      \"Self-signed certificates are not accepted and submission of a self-signed SSL certificate\n      will delay the approval of your registration.\"\n    evidence:\n      - url: https://api.pge.com/GreenButtonConnect/espi/1_1/resource/Authorization\n        status: 400\n        body: '\"Invalid Certificate\"'\n        fetched: '2026-09-17'\n      - url: https://api.pge.com/GreenButtonConnect/espi/1_1/resource/ReadServiceStatus\n        status: 400\n    \
  \    body: '\"Invalid Certificate\"'\n        fetched: '2026-09-17'\n    source: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: client_credentials\n        tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n        token_class: client_access_token\n        description: >-\n          Third-party-level token. Used for the third party's own resources — ApplicationInformation,\n          the Authorization feed, ReadServiceStatus, and every Bulk resource\n          (Batch/Bulk/{BulkID}, Batch/BulkRetailCustomerInfo/{BulkID},\n          Batch/BulkRetailDRPrgInfo/{BulkID}).\n      - flow: authorization_code\n        authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/Authorize\n        tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n        token_class: access_token\n        description: >-\n          Per-customer token, issued after a PG&E customer\
  \ authenticates on PG&E's own site and\n          chooses what to share. Used for every customer-scoped resource under\n          Subscription/{SubscriptionID}/... . Paired with a refresh token.\n      - flow: refresh_token\n        tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n        description: Refreshes the per-customer access token.\n    scope_format: ESPI function-block string — see scopes/pg-and-e-scopes.yml\n    revocation:\n      operation: DELETE /GreenButtonConnect/espi/1_1/resource/Authorization/{AuthorizationID}\n      token: client_access_token\n      description: Cancels an individual customer authorization.\n    evidence:\n      - url: https://api.pge.com/datacustodian/oauth/v2/token\n        method: GET\n        status: 405\n        body: '{\"error\":\"invalid_request\",\"error_description\":\"GET not permitted\"}'\n        fetched: '2026-09-17'\n      - url: https://api.pge.com/datacustodian/test/oauth/v2/token\n        method: GET\n        status: 400\n\
  \        body: '{\"error\":\"invalid_request\",\"error_description\":\"Missing grant_type\"}'\n        fetched: '2026-09-17'\n      - url: https://api.pge.com/datacustodian/test/oauth/v2/authorize\n        method: GET\n        status: 400\n        body: '{\"error\":\"invalid_request\",\"error_description\":\"client_id is empty\"}'\n        fetched: '2026-09-17'\n    sources:\n      - https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/OAuth_Authorization_ESPI.pdf\n      - https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-APIs.pdf\nonboarding:\n  self_serve: false\n  gate: application approval by PG&E under the CPUC framework\n  registration_url: https://sharemydata.pge.com/\n  prerequisites:\n    - A 9-digit U.S. Employer Identification Number (EIN)\n    - Business and technical contacts\n    - A third-party notification URI for the ESPI push (FB 39) model\n    - A CA-issued TLS 1.2 X.509 certificate (self-signed rejected)\n\
  \  source: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\nsupport: mailto:ShareMyData@pge.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/authentication/pg-and-e-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Energy
- Utilities
- Electricity
- Natural Gas
- California
- United States
- Smart Metering
- Green Button
- ESPI
- Energy Usage Data
- Investor-Owned Utility
- Customer Data Access
---
