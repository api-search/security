---
anonymous_access: false
api_key_in:
- body
- header
api_specs:
- filename: sofi-technologies-program-api-openapi.json
  format: json
  label: SoFi Tech Solutions Program API
  slug: sofi-tech-solutions-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-program-api-openapi.json
- filename: sofi-technologies-payment-hub-api-openapi.json
  format: json
  label: SoFi Tech Solutions Payment Hub API 2.0
  slug: sofi-tech-solutions-payment-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-payment-hub-api-openapi.json
- filename: sofi-technologies-dispute-api-3-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 3.0
  slug: sofi-tech-solutions-dispute-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-3-0-openapi.json
- filename: sofi-technologies-dispute-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 2.0
  slug: sofi-tech-solutions-dispute-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-2-0-openapi.json
- filename: sofi-technologies-loan-api-openapi.json
  format: json
  label: SoFi Tech Solutions Loan API
  slug: sofi-tech-solutions-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-loan-api-openapi.json
- filename: sofi-technologies-risk-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 2.0
  slug: sofi-tech-solutions-risk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-2-0-openapi.json
- filename: sofi-technologies-risk-api-1-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 1.0
  slug: sofi-tech-solutions-risk-api-10
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-1-0-openapi.json
- filename: sofi-technologies-public-config-api-openapi.json
  format: json
  label: SoFi Tech Solutions Public Config API
  slug: sofi-tech-solutions-public-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-public-config-api-openapi.json
- filename: sofi-technologies-events-api-openapi.json
  format: json
  label: SoFi Tech Solutions Events API
  slug: sofi-tech-solutions-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-events-api-openapi.json
- filename: sofi-technologies-auth-api-openapi.json
  format: json
  label: SoFi Tech Solutions Auth API
  slug: sofi-tech-solutions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-auth-api-openapi.json
- filename: sofi-technologies-external-trans-api-openapi.json
  format: json
  label: SoFi Tech Solutions External Trans API
  slug: sofi-tech-solutions-external-trans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-external-trans-api-openapi.json
auth_types:
- body-parameter
- http-bearer
- apiKey
description: Authentication on the SoFi Tech Solutions platform is split three ways, and the largest surface is the one the specifications do not describe. A mechanical derivation from openapi/ finds only two bearer-style schemes, on the Loan and Risk APIs; it finds nothing at all on the 167-operation Program API, because that API authenticates with credentials carried as ordinary form parameters in the request body and declares no securityScheme. This artifact was upgraded from that thin derivation by reading the provider's Authentication reference page.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Sofi Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: SoFi Technologies secures its APIs with body-parameter, http-bearer, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SoFi Technologies
provider_slug: sofi-technologies
scheme_count: 3
schemes:
- content_type: application/x-www-form-urlencoded
  declared_in_spec: false
  failure_codes:
  - code: 4
    meaning: Failed API login
  - code: 18
    meaning: Unauthorized access to this version of the API
  - code: 21
    meaning: Unregistered IP address
  - code: 29
    meaning: Incorrect provider ID
  - code: 50
    meaning: Invalid JWT
  ip_binding: true
  ip_binding_note: Credentials are issued for a specific requesting IP address. A call from an unregistered IP returns status_code 21. This is a meaningful second factor - a leaked apiLogin/apiTransKey is not usable from an arbitrary host - and it is also why these APIs cannot be called from ephemeral or serverless egress without coordination.
  name: program-api-credentials
  parameters:
  - description: Username for the requesting IP address, provided by SoFi Tech Solutions
    max_length: 50
    name: apiLogin
    required: true
    type: string
  - description: Password for the requesting IP address, provided by SoFi Tech Solutions
    max_length: 15
    name: apiTransKey
    required: true
    type: string
  - description: Provider identifier from SoFi Tech Solutions
    max_digits: 10
    name: providerId
    required: true
    type: integer
  - description: Caller-generated per-request id, UUID preferred; also the idempotency key on 35 endpoints
    max_length: 60
    name: transactionId
    required: true
    type: string
  - description: Optional caller id for internal reporting; echoed back
    max_length: 60
    name: providerTransactionId
    required: false
    type: string
  - description: Optional caller timestamp; echoed back
    format: YYYY-MM-DD hh:mm:ss
    name: providerTimestamp
    required: false
    type: date-time
  rotation: Sandbox credentials must be regenerated every 30 days by the company's Sandbox team admin; stale details fail the request and can lock the company account. No rotation policy is published for Client Validation or Production.
  surface: Program API 4.0 (167 operations) - and the platform's default
  transport: HTTPS; TLS 1.2 minimum, TLS 1.3 strongly recommended
  type: body-parameter
- bearerFormat: JWT
  declared_in_spec: true
  name: bearerAuth
  note: On the Auth API this secures the CLIENT's webhook endpoint - SoFi Tech Solutions is the caller presenting the token, not the other way round. On the Risk APIs the scheme name in the contract is gft-internal-service-auth.
  scheme: bearer
  sources:
  - openapi/sofi-technologies-auth-api-openapi.json
  - openapi/sofi-technologies-risk-api-1-0-openapi.json
  - openapi/sofi-technologies-risk-api-2-0-openapi.json
  type: http
- declared_in_spec: true
  in: header
  name: BearerAuth
  note: Modelled as an apiKey in the Authorization header rather than as http/bearer, and its description carries an unresolved "[here](link)" placeholder - the contract points at documentation that was never linked.
  parameter: Authorization
  sources:
  - openapi/sofi-technologies-loan-api-openapi.json
  spec_description: 'Authorization header is required for requests


    For more information click [here](link)'
  type: apiKey
slug: sofi-technologies-authentication
source_filename: sofi-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: SoFi Technologies\nproviderId: sofi-technologies\ngenerated: '2026-09-06'\nmethod: searched\nsource: https://docs.tech.sofi.com/pro/reference/api-reference-authentication\ndocs:\n  - https://docs.tech.sofi.com/pro/reference/api-reference-authentication\n  - https://docs.tech.sofi.com/pro/docs/quickstart\n  - https://docs.tech.sofi.com/pro/docs/environments\n  - https://docs.tech.sofi.com/pro/docs/sofi-tech-solutions-tools\ndescription: >-\n  Authentication on the SoFi Tech Solutions platform is split three ways, and the largest surface\n  is the one the specifications do not describe. A mechanical derivation from openapi/ finds only\n  two bearer-style schemes, on the Loan and Risk APIs; it finds nothing at all on the 167-operation\n  Program API, because that API authenticates with credentials carried as ordinary form parameters\n  in the request body and declares no securityScheme. This artifact\
  \ was upgraded from that thin\n  derivation by reading the provider's Authentication reference page.\nsummary:\n  types: [body-parameter, http-bearer, apiKey]\n  api_key_in: [body, header]\n  oauth2: false\n  openid_connect_for_api: false\n  mtls: false\n  spec_declares_program_api_auth: false\nschemes:\n  - name: program-api-credentials\n    type: body-parameter\n    surface: Program API 4.0 (167 operations) - and the platform's default\n    declared_in_spec: false\n    parameters:\n      - { name: apiLogin, required: true, type: string, max_length: 50, description: 'Username for the requesting IP address, provided by SoFi Tech Solutions' }\n      - { name: apiTransKey, required: true, type: string, max_length: 15, description: 'Password for the requesting IP address, provided by SoFi Tech Solutions' }\n      - { name: providerId, required: true, type: integer, max_digits: 10, description: 'Provider identifier from SoFi Tech Solutions' }\n      - { name: transactionId, required: true,\
  \ type: string, max_length: 60, description: 'Caller-generated per-request id, UUID preferred; also the idempotency key on 35 endpoints' }\n      - { name: providerTransactionId, required: false, type: string, max_length: 60, description: 'Optional caller id for internal reporting; echoed back' }\n      - { name: providerTimestamp, required: false, type: date-time, format: 'YYYY-MM-DD hh:mm:ss', description: 'Optional caller timestamp; echoed back' }\n    content_type: application/x-www-form-urlencoded\n    transport: HTTPS; TLS 1.2 minimum, TLS 1.3 strongly recommended\n    ip_binding: true\n    ip_binding_note: >-\n      Credentials are issued for a specific requesting IP address. A call from an unregistered IP\n      returns status_code 21. This is a meaningful second factor - a leaked apiLogin/apiTransKey\n      is not usable from an arbitrary host - and it is also why these APIs cannot be called from\n      ephemeral or serverless egress without coordination.\n    rotation: >-\n \
  \     Sandbox credentials must be regenerated every 30 days by the company's Sandbox team admin;\n      stale details fail the request and can lock the company account. No rotation policy is\n      published for Client Validation or Production.\n    failure_codes:\n      - { code: 4, meaning: Failed API login }\n      - { code: 18, meaning: Unauthorized access to this version of the API }\n      - { code: 21, meaning: Unregistered IP address }\n      - { code: 29, meaning: Incorrect provider ID }\n      - { code: 50, meaning: Invalid JWT }\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    declared_in_spec: true\n    sources:\n      - openapi/sofi-technologies-auth-api-openapi.json\n      - openapi/sofi-technologies-risk-api-1-0-openapi.json\n      - openapi/sofi-technologies-risk-api-2-0-openapi.json\n    note: >-\n      On the Auth API this secures the CLIENT's webhook endpoint - SoFi Tech Solutions is the\n      caller presenting the token, not the\
  \ other way round. On the Risk APIs the scheme name in\n      the contract is gft-internal-service-auth.\n  - name: BearerAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    declared_in_spec: true\n    sources: [openapi/sofi-technologies-loan-api-openapi.json]\n    spec_description: |-\n      Authorization header is required for requests\n\n      For more information click [here](link)\n    note: >-\n      Modelled as an apiKey in the Authorization header rather than as http/bearer, and its\n      description carries an unresolved \"[here](link)\" placeholder - the contract points at\n      documentation that was never linked.\nconsole_sso:\n  applies_to: the SoFi Tech Solutions web tools (Console, Config, CST, gAnalytics, Client Portal)\n  applies_to_api: false\n  mechanism: SSO from the client's own enterprise identity provider\n  supported_idps: [Okta, Microsoft Entra ID, Google, 'any OpenID Connect provider']\n  note: >-\n    OIDC is used to sign humans into the\
  \ consoles. It is NOT an API authorization mechanism and no\n    /.well-known/openid-configuration is served on any SoFi host - see\n    well-known/sofi-technologies-well-known.yml.\n  docs: https://docs.tech.sofi.com/pro/docs/sofi-tech-solutions-tools\noauth_scopes:\n  published: false\n  note: >-\n    No OAuth 2.0 anywhere on the API surface, therefore no scopes. derive-oauth-scopes.py found\n    zero oauth2 securitySchemes across the 11 definitions and no scopes artifact was written.\ngaps:\n  - >-\n    The platform's primary authentication mechanism is invisible to any tool that reads the\n    OpenAPI. A client generated from openapi/sofi-technologies-program-api-openapi.json will not\n    send credentials at all.\n  - >-\n    Credentials travel in the request body rather than in a header, so they land in any\n    intermediary that logs request bodies, and they cannot be scoped, expired or revoked\n    independently of the account.\n  - No published rotation policy for production credentials.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/authentication/sofi-technologies-authentication.yml
summary_line: body-parameter/http-bearer/apiKey · 3 schemes
tags:
- Fintech
- Payments
- Banking
- Card Issuing
- Banking as a Service
- Personal Finance
- Lending
- ACH
- ISO 20022
- Disputes
- Identity Verification
- Webhooks
---
