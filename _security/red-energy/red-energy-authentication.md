---
api_key_in: []
api_specs:
- filename: red-energy-cds-energy-openapi.yml
  format: yaml
  label: Red Energy CDR Energy Product Reference Data API
  slug: red-energy-cdr-energy-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-cds-energy-openapi.yml
- filename: red-energy-cds-common-openapi.yml
  format: yaml
  label: Red Energy CDR Discovery API
  slug: red-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-cds-common-openapi.yml
- filename: red-energy-cds-energy-openapi.yml
  format: yaml
  label: Red Energy CDR Energy Consumer Data API
  slug: red-energy-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-cds-energy-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Red Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Red Energy secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Red Energy
provider_slug: red-energy
scheme_count: 4
schemes:
- applies_to:
  - listEnergyPlans
  - getEnergyPlanDetail
  - getStatus
  - getOutages
  description: Unauthenticated public endpoints. Under the CDS these MUST NOT use mutual TLS; they are served over ordinary one-way TLS.
  name: none
  sources:
  - openapi/red-energy-cds-energy-openapi.yml
  - openapi/red-energy-cds-common-openapi.yml
  type: none
- flows:
  - authorizationUrl: null
    description: Authorization Code flow with PKCE (S256). The CDS also documents the OIDC Hybrid flow; Authorization Code flow is the current profile for FAPI 1.0 Final Phase 3 obligations.
    flow: authorizationCode
    tokenUrl: null
    url_note: Per-data-holder endpoints are advertised in the data holder's OpenID Provider Configuration document, which is published only to accredited participants. Red Energy's is not anonymously discoverable.
  name: CDR OAuth2 / OpenID Connect (FAPI 1.0 Advanced)
  profile: FAPI 1.0 Advanced (OpenID Foundation Financial-grade API)
  requires:
    client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
    client_authentication: private_key_jwt
    consent: Explicit, scoped, time-limited consumer authorisation. A CDR-mandated consumer dashboard lets the customer review, amend and withdraw sharing at any time.
    id_token_signing_alg:
    - ES256
    - PS256
    pkce: S256
    pushed_authorisation_requests: true
    request_object: signed JWT (ES256 or PS256)
    sender_constrained_tokens: mutual-TLS holder-of-key — tls_client_certificate_bound_access_tokens true. Resource requests MUST be validated so the client certificate and the access token match. OAUTB is not supported.
    subject_identifier: pairwise (PPID), RECOMMENDED as a UUID v4
  scopes_artifact: scopes/red-energy-scopes.yml
  type: oauth2
- certificate_profile:
    common_name: primary DNS name (server) / software product name (client)
    key_algorithm: RSA
    key_size: 2048
    organizational_unit: Consumer Data Right
    signature_algorithm: SHA256
  ciphers: From 17 March 2025 the FAPI 1.0 Advanced TLS considerations apply. Prior to that only TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 and TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 were permitted.
  description: All back-channel traffic between an accredited data recipient and a data holder uses mTLS. Both client and server transport certificates MUST be issued by the CDR Certificate Authority; certificates from any other authority MUST NOT be trusted.
  name: CDR mutual TLS
  type: mutualTLS
- description: Each data holder publishes /.well-known/openid-configuration on its TLS base URI with acr_values_supported urn:cds.au:cdr:2 and urn:cds.au:cdr:3, require_pushed_authorization_requests true, a cdr_arrangement_revocation_endpoint, and token_endpoint_auth_methods_supported private_key_jwt.
  name: CDR OpenID Provider Configuration
  openIdConnectUrl: null
  probe:
    date: '2026-07-27'
    status: 404
    url: https://public.cdr.redenergy.com.au/.well-known/openid-configuration
  type: openIdConnect
slug: red-energy-authentication
source_filename: red-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://consumerdatastandardsaustralia.github.io/standards/#security-profile —\n  the Consumer Data Standards (CDS) Security Profile, v1.36.0. Red Energy\n  publishes no authentication documentation of its own; as a designated CDR\n  energy data holder its authentication contract IS the CDS Security Profile.\n  The mechanical derivation from the harvested OpenAPI produced nothing: the DSB\n  cds_energy and cds_common documents declare no components.securitySchemes at\n  all, expressing per-operation authorisation only through the x-scopes vendor\n  extension. This profile therefore comes from the standard's prose, plus what\n  was observed live on 2026-07-27.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nprovider: Red Energy\nproviderId: red-energy\n\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n \
  \   Two distinct authentication postures on one provider. The anonymous half\n    (Product Reference Data + Data Holder Operations discovery) takes no\n    credential at all. The consumer-authorised half takes the full FAPI 1.0\n    Advanced stack and is reachable only by an ACCC-accredited data recipient.\n\nsurfaces:\n  - name: CDR Energy Product Reference Data (anonymous)\n    base_url: https://cdr.energymadeeasy.gov.au/red-energy/cds-au/v1\n    operations: [listEnergyPlans, getEnergyPlanDetail]\n    auth: none\n    verified: >-\n      HTTP 200 with no credential on 2026-07-27. No API key, no signup, no\n      terms click-through, no registration.\n    required_headers:\n      - name: x-v\n        required: true\n        description: >-\n          Endpoint payload version. Mandatory on every CDS endpoint. Omitting it\n          returns 400 urn:au-cds:error:cds-all:Header/Missing.\n      - name: x-min-v\n        required: false\n        description: Minimum acceptable endpoint version\
  \ for negotiation.\n  - name: CDR Common Data Holder Operations (anonymous)\n    base_url: https://public.cdr.redenergy.com.au/cds-au/v1\n    operations: [getStatus, getOutages]\n    auth: none\n    verified: HTTP 200 with no credential on 2026-07-27.\n  - name: CDR Energy + Common consumer data (accredited only)\n    base_url: null\n    base_url_note: >-\n      The data holder's infosec and mTLS base URIs are published only through\n      the AUTHENTICATED portion of the CDR Register. GET\n      https://public.cdr.redenergy.com.au/.well-known/openid-configuration\n      returned HTTP 404 (nginx) on 2026-07-27 — no anonymous OIDC discovery\n      document exists on the public base URI.\n    operations:\n      - getCustomer\n      - getCustomerDetail\n      - listEnergyAccounts\n      - getEnergyAccountDetail\n      - getEnergyAccountBalance\n      - listEnergyAccountBalancesBulk\n      - listEnergyAccountBalancesSpecificAccounts\n      - getBillingForEnergyAccount\n      - listEnergyAccountBillingBulk\n\
  \      - listEnergyAccountBillingForSpecificAccounts\n      - getEnergyAccountInvoices\n      - listEnergyAccountInvoicesBulk\n      - listEnergyInvoicesForSpecificAccounts\n      - getEnergyAccountConcessions\n      - getEnergyAccountPaymentSchedule\n      - listElectricityServicePoints\n      - getElectricityServicePointDetail\n      - listElectricityUsageBulk\n      - getElectricityServicePointUsage\n      - listElectricityUsageForServicePoints\n      - listElectricityDERBulk\n      - getElectricityDERForServicePoint\n      - listElectricityDERForSpecificServicePoints\n    auth: oauth2 + openIdConnect over mutualTLS\n    verified: false\n    verified_note: >-\n      Not called. Accreditation, CDR Register-issued certificates and a consented\n      authorisation are required; the surface is unreachable from outside the\n      regime by design. The obligation is confirmed by the CDR Register listing.\n\nschemes:\n  - name: none\n    type: none\n    applies_to: [listEnergyPlans, getEnergyPlanDetail,\
  \ getStatus, getOutages]\n    sources: [openapi/red-energy-cds-energy-openapi.yml, openapi/red-energy-cds-common-openapi.yml]\n    description: >-\n      Unauthenticated public endpoints. Under the CDS these MUST NOT use mutual\n      TLS; they are served over ordinary one-way TLS.\n  - name: CDR OAuth2 / OpenID Connect (FAPI 1.0 Advanced)\n    type: oauth2\n    profile: FAPI 1.0 Advanced (OpenID Foundation Financial-grade API)\n    flows:\n      - flow: authorizationCode\n        description: >-\n          Authorization Code flow with PKCE (S256). The CDS also documents the\n          OIDC Hybrid flow; Authorization Code flow is the current profile for\n          FAPI 1.0 Final Phase 3 obligations.\n        authorizationUrl: null\n        tokenUrl: null\n        url_note: >-\n          Per-data-holder endpoints are advertised in the data holder's OpenID\n          Provider Configuration document, which is published only to accredited\n          participants. Red Energy's is not anonymously\
  \ discoverable.\n    requires:\n      pushed_authorisation_requests: true\n      request_object: signed JWT (ES256 or PS256)\n      pkce: S256\n      client_authentication: private_key_jwt\n      client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n      sender_constrained_tokens: >-\n        mutual-TLS holder-of-key — tls_client_certificate_bound_access_tokens\n        true. Resource requests MUST be validated so the client certificate and\n        the access token match. OAUTB is not supported.\n      subject_identifier: pairwise (PPID), RECOMMENDED as a UUID v4\n      id_token_signing_alg: [ES256, PS256]\n      consent: >-\n        Explicit, scoped, time-limited consumer authorisation. A CDR-mandated\n        consumer dashboard lets the customer review, amend and withdraw sharing\n        at any time.\n    scopes_artifact: scopes/red-energy-scopes.yml\n  - name: CDR mutual TLS\n    type: mutualTLS\n    description: >-\n      All back-channel traffic between\
  \ an accredited data recipient and a data\n      holder uses mTLS. Both client and server transport certificates MUST be\n      issued by the CDR Certificate Authority; certificates from any other\n      authority MUST NOT be trusted.\n    certificate_profile:\n      signature_algorithm: SHA256\n      key_algorithm: RSA\n      key_size: 2048\n      organizational_unit: Consumer Data Right\n      common_name: primary DNS name (server) / software product name (client)\n    ciphers: >-\n      From 17 March 2025 the FAPI 1.0 Advanced TLS considerations apply. Prior to\n      that only TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 and\n      TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 were permitted.\n  - name: CDR OpenID Provider Configuration\n    type: openIdConnect\n    openIdConnectUrl: null\n    description: >-\n      Each data holder publishes /.well-known/openid-configuration on its TLS\n      base URI with acr_values_supported urn:cds.au:cdr:2 and urn:cds.au:cdr:3,\n      require_pushed_authorization_requests\
  \ true, a cdr_arrangement_revocation_endpoint,\n      and token_endpoint_auth_methods_supported private_key_jwt.\n    probe:\n      url: https://public.cdr.redenergy.com.au/.well-known/openid-configuration\n      status: 404\n      date: '2026-07-27'\n\ntokens:\n  access_token: >-\n    Lifetime MUST be deterministic and returned in expires_in on the token\n    response. Sender-constrained to the client's mTLS certificate.\n  refresh_token: >-\n    Issued for ongoing (unattended) sharing; bounded by the consent duration and\n    revocable through the consumer dashboard or the CDR arrangement revocation\n    endpoint.\n\naccreditation:\n  regulator: Australian Competition and Consumer Commission (ACCC)\n  register: https://api.cdr.gov.au/cdr-register/v1/energy/data-holders/brands/summary\n  data_holder_brand_id: 39230258-a56c-ee11-a81c-002248e31327\n  public_base_uri: https://public.cdr.redenergy.com.au\n  pathways:\n    - unrestricted accreditation\n    - sponsored accreditation\n    -\
  \ CDR representative\n    - trusted adviser\n  steps: >-\n    Apply to the ACCC, obtain CDR Register client credentials and transport and\n    signing certificates from the CDR Certificate Authority, pass Conformance\n    Test Suite testing, then initiate a consent flow the individual Red Energy\n    customer approves. There is no self-serve path and no commercial API deal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/authentication/red-energy-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Open Data
---
