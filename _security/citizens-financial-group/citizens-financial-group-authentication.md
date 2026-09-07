---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: citizens-financial-group-accounts-openapi.yml
  format: yaml
  label: Citizens Accounts API
  slug: citizens-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-accounts-openapi.yml
- filename: citizens-financial-group-statements-openapi.yml
  format: yaml
  label: Citizens Statements API
  slug: citizens-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-statements-openapi.yml
- filename: citizens-financial-group-payments-openapi.yml
  format: yaml
  label: Citizens Payments API
  slug: citizens-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-payments-openapi.yml
- filename: citizens-financial-group-account-validation-openapi.yml
  format: yaml
  label: Citizens Account Validation API
  slug: citizens-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-validation-openapi.yml
- filename: citizens-financial-group-account-transfer-openapi.yml
  format: yaml
  label: Citizens Account Transfer API
  slug: citizens-account-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-transfer-openapi.yml
- filename: citizens-financial-group-information-reporting-openapi.yml
  format: yaml
  label: Citizens Information Reporting API
  slug: citizens-information-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-information-reporting-openapi.yml
- filename: citizens-financial-group-authorize-openapi.yml
  format: yaml
  label: Citizens Authorize API
  slug: citizens-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-authorize-openapi.yml
- filename: citizens-financial-group-atm-locator-openapi.yml
  format: yaml
  label: Citizens ATM Locator API
  slug: citizens-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-atm-locator-openapi.yml
- filename: citizens-financial-group-branch-locator-openapi.yml
  format: yaml
  label: Citizens Branch Locator API
  slug: citizens-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-branch-locator-openapi.yml
auth_types:
- oauth2
- apiKey
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Citizens Financial Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Citizens Financial Group secures its APIs with oauth2, apiKey, and mutualTLS across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Citizens Financial Group
provider_slug: citizens-financial-group
scheme_count: 5
schemes:
- applies_to:
  - Payments
  - Account Transfer
  - Account Validation
  - Information Reporting
  flow: clientCredentials
  name: OAuth2
  sources:
  - openapi/citizens-financial-group-payments-openapi.yml
  - openapi/citizens-financial-group-account-transfer-openapi.yml
  - openapi/citizens-financial-group-account-validation-openapi.yml
  - openapi/citizens-financial-group-information-reporting-openapi.yml
  type: oauth2
- applies_to:
  - Payments
  - Account Transfer
  - Account Validation
  - Information Reporting
  description: IBM API Connect application client id (called "API Key" in the portal). Retrieved from Apps > your application > Subscriptions in the developer portal.
  in: header
  name: client-id
  parameter: X-IBM-Client-Id
  type: apiKey
- applies_to:
  - Accounts (FDX v1.0 and v2.1)
  - Statements (FDX v1.0 and v2.1)
  description: Identifies the desired financial institution or partners.
  in: header
  name: x-fapi-financial-id
  parameter: x-fapi-financial-id
  type: apiKey
- applies_to:
  - Authorize (IDP v1.0 / v2.0)
  description: Identifies the desired financial institution or partners.
  in: header
  name: x-client-id
  parameter: x-client-id
  type: apiKey
- applies_to:
  - ATM Locator
  - Branch Locator
  description: Used for differentiating the registered vendors/partners.
  in: header
  name: Partner Id
  parameter: Partner-ID
  type: apiKey
slug: citizens-financial-group-authentication
source_filename: citizens-financial-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf (v1.3, updated\n  2025-12-11) section 3 \"AUTHENTICATION\"; the same section appears in the Account Transfer (v1.0,\n  2026-05-29), Account Validation (v1.6, 2026-04-30) and Information Reporting (v1.6, 2026-07-22)\n  user guides. Scheme detail derived from the harvested specs in openapi/.\ndocs: https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf\nprovider: Citizens Financial Group\nproviderId: citizens-financial-group\n\nsummary:\n  model: >-\n    Two-legged OAuth 2.0 client-credentials with a private_key_jwt client assertion over mutual TLS,\n    stated by Citizens to follow the Financial-grade API (FAPI) Security Profile 1.0 - Part 2:\n    Advanced. Every commercial-banking call additionally carries an IBM API Connect client id header\n    (X-IBM-Client-Id) issued by the developer portal, and a required x-fapi-trace-id\
  \ correlation\n    header. The FDX account/statement surface and the ATM/branch locator surface are key-header only\n    in the published contracts.\n  types:\n    - oauth2\n    - apiKey\n    - mutualTLS\n  api_key_in:\n    - header\n  oauth2_flows:\n    - clientCredentials\n\ntoken_endpoints:\n  - environment: production\n    url: https://apis.citizensbank.com/as/token.oauth2\n    source: CitizensPaymentAPIUserGuide.pdf section 3.1.3\n  - environment: sandbox\n    url: https://sandboxapis.citizensbank.com/as/token.oauth2\n    source: CitizensPaymentAPIUserGuide.pdf section 3.1.3\n  - environment: production (JWT `aud` claim value)\n    url: https://pf-fam.citizensbank.com\n    source: CitizensPaymentAPIUserGuide.pdf section 3.1.2\n  - environment: sandbox (JWT `aud` claim value)\n    url: https://pf-fam-sb.internal.citizensbank.com\n    source: CitizensPaymentAPIUserGuide.pdf section 3.1.2\n  - environment: as published in the OpenAPI securitySchemes\n    url: https://pf-fam.internal.citizensbank.com/as/token.oauth2\n\
  \    source: openapi/_original/citizens-payments-v3.json\n    note: >-\n      The tokenUrl carried in the specs' oauth2 securityScheme names an .internal. host that does not\n      resolve publicly; the user guides publish apis.citizensbank.com / sandboxapis.citizensbank.com\n      as the callable token endpoints. Recorded as-published, not reconciled.\n\nflow:\n  name: OAuth 2.0 JWT client assertion (private_key_jwt) over mTLS\n  grant_type: client_credentials\n  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n  steps:\n    - Client and Citizens authorization server present certificates validated against a shared CA (mTLS).\n    - Client builds a JWT assertion with iss = sub = Client ID from the developer portal, aud = the\n      token endpoint URL, exp <= 3600 seconds, and a unique jti to prevent replay.\n    - JWT is signed with the client private key (RS256); the client hosts a JWKS URL exposing the\n      public key for Citizens to verify.\n    - Client\
  \ POSTs client_id, grant_type, client_assertion_type, client_assertion and scope to the\n      token endpoint over the mTLS channel.\n    - Citizens validates the assertion and the client certificate and issues a Bearer access token.\n    - Client calls the resource server with the Bearer token plus X-IBM-Client-Id and x-fapi-trace-id.\n  jwt_claims:\n    - iss (Client ID from the developer portal)\n    - sub (same as iss)\n    - aud (token endpoint URL)\n    - exp (must not exceed 3600 seconds)\n    - jti (unique, to prevent replay)\n  signing_algorithm: RS256\n  client_key_distribution: JWKS endpoint hosted by the client, or a key store supplied at onboarding\n  mutual_tls: true\n  ip_allowlisting: >-\n    Client IPs are provisioned by the Citizens Implementation Manager during onboarding\n    (CitizensPaymentAPIUserGuide.pdf section 2).\n\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: clientCredentials\n    applies_to:\n      - Payments\n      - Account Transfer\n      - Account\
  \ Validation\n      - Information Reporting\n    sources:\n      - openapi/citizens-financial-group-payments-openapi.yml\n      - openapi/citizens-financial-group-account-transfer-openapi.yml\n      - openapi/citizens-financial-group-account-validation-openapi.yml\n      - openapi/citizens-financial-group-information-reporting-openapi.yml\n  - name: client-id\n    type: apiKey\n    in: header\n    parameter: X-IBM-Client-Id\n    description: >-\n      IBM API Connect application client id (called \"API Key\" in the portal). Retrieved from\n      Apps > your application > Subscriptions in the developer portal.\n    applies_to:\n      - Payments\n      - Account Transfer\n      - Account Validation\n      - Information Reporting\n  - name: x-fapi-financial-id\n    type: apiKey\n    in: header\n    parameter: x-fapi-financial-id\n    description: Identifies the desired financial institution or partners.\n    applies_to:\n      - Accounts (FDX v1.0 and v2.1)\n      - Statements (FDX v1.0 and\
  \ v2.1)\n  - name: x-client-id\n    type: apiKey\n    in: header\n    parameter: x-client-id\n    description: Identifies the desired financial institution or partners.\n    applies_to:\n      - Authorize (IDP v1.0 / v2.0)\n  - name: Partner Id\n    type: apiKey\n    in: header\n    parameter: Partner-ID\n    description: Used for differentiating the registered vendors/partners.\n    applies_to:\n      - ATM Locator\n      - Branch Locator\n\nrequired_headers:\n  - name: x-fapi-trace-id\n    required: true\n    max_length: 36\n    description: Unique request id (UUID) for each request to make it traceable.\n  - name: x-fapi-channel-id\n    required: false\n    max_length: 20\n    description: Distinguishes communication channels or data streams within a client system.\n  - name: Authorization\n    required: true\n    description: OAuth 2.0 Bearer access token.\n  - name: X-IBM-Client-Id\n    required: true\n    description: Developer-portal application client id.\n  - name: requestid\n\
  \    required: false\n    max_length: 36\n    description: >-\n      Consumer-assigned request identifier echoed back as requestId for tracking, logging and\n      correlation (Payments user guide 5.1.2 / 5.1.5).\n\nonboarding:\n  process: >-\n    Access is not self-service. A Citizens Implementation Manager runs a kickoff, collects authorized\n    security contacts, the client IPs to allowlist, the public key for the mTLS certificate and a\n    private key via JWKS endpoint or key store. All testing happens in the sandbox; message signing\n    and sandbox sign-off are required before a production date is agreed and the application is\n    registered by the Citizens API team.\n  portal_roles:\n    - Owner - manages organization settings, applications and credentials; may invite additional users.\n    - Administrator - same permissions as owner.\n    - Developer - view/manage organization settings, application settings/credentials, subscriptions, analytics.\n    - Viewer - view-only access\
  \ to organization, applications and analytics.\n  source: https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf\n\nnotes:\n  - No public OpenID Connect discovery document is served; /.well-known/openid-configuration on every\n    Citizens host probed on 2026-09-05 either 404s or returns the portal search page (see well-known/).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/authentication/citizens-financial-group-authentication.yml
summary_line: oauth2/apiKey/mutualTLS · 5 schemes
tags:
- Banking
- Buy Now Pay Later
- Financial-Services
- FDX
- Locator
- Open Banking
- Payments
---
