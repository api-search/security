---
api_key_in: []
api_specs:
- filename: energy-queensland-data-holder-customers-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Customers API
  slug: energy-queensland-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-customers-api-openapi.yml
- filename: energy-queensland-data-holder-operations-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Operations API
  slug: energy-queensland-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-operations-api-openapi.yml
- filename: energy-queensland-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Energy Queensland Distributed Energy Resources API
  slug: energy-queensland-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-distributed-energy-resources-api-openapi.yml
- filename: energy-queensland-electricity-service-points-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Service Points API
  slug: energy-queensland-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-service-points-api-openapi.yml
- filename: energy-queensland-electricity-usage-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Usage API
  slug: energy-queensland-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-usage-api-openapi.yml
- filename: energy-queensland-energy-account-balances-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Balances API
  slug: energy-queensland-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-balances-api-openapi.yml
- filename: energy-queensland-energy-account-billing-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Billing API
  slug: energy-queensland-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-billing-api-openapi.yml
- filename: energy-queensland-energy-accounts-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Accounts API
  slug: energy-queensland-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-accounts-api-openapi.yml
- filename: energy-queensland-energy-plans-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Plans API
  slug: energy-queensland-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-plans-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: 'Energy Queensland''s API estate has exactly two authentication postures, and the line between them is statutory rather than commercial. Everything a member of the public can reach is completely unauthenticated - no key, no signup, no terms click-through, only an x-v version header. Everything about an identifiable customer is behind the full Consumer Data Right security profile: ACCC accreditation, mutual TLS with CDR Register-issued certificates, FAPI 1.0 Advanced OAuth2 with private_key_jwt client authentication, OIDC, and per-consumer consent. There is no middle tier, no partner key, no commercial API deal, and no self-serve credential of any kind. NOTE ON PROVENANCE: the harvested OpenAPI documents declare NO securitySchemes at all (components.securitySchemes is empty in both cds_energy 1.36.0 and cds_common 1.36.0) because the DSB publishes the security model in the Security Profile section of the standard rather than in the swagger. This profile was therefore read from
  the standard and from live behaviour, not derived by 0-working/derive-authentication.py, which found nothing to derive.'
kind: authentication
layout: security
method: searched
name: Energy Queensland Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Energy Queensland secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Energy Queensland
provider_slug: energy-queensland
scheme_count: 4
schemes:
- applies_to:
  - listEnergyPlans
  - getEnergyPlanDetail
  - getStatus
  - getOutages
  evidence: 'GET https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1/energy/plans with only "x-v: 1" returned HTTP 200 with 36 Ergon plans on 2026-07-27, and GET https://public.cdr.ergonretail.com.au/cds-au/v1/discovery/status returned HTTP 200 status OK. No credential of any kind was sent.'
  hosts:
  - https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1
  - https://public.cdr.ergonretail.com.au/cds-au/v1
  name: none (public CDR surface)
  optional_headers:
  - description: Minimum acceptable endpoint version.
    name: x-min-v
  - description: RFC 4122 UUID correlation id. Played back verbatim in the response - verified live 2026-07-27 against the AER-hosted plans endpoint.
    name: x-fapi-interaction-id
  required_headers:
  - description: Requested endpoint version. Mandatory. Omitting it returns HTTP 400 urn:au-cds:error:cds-all:Header/Missing - verified live 2026-07-27.
    name: x-v
    required: true
  type: none
- applies_to: all consumer-authorised energy and common operations
  certificate_authority: CDR Register (ACCC) private CA - transport and signing certificates
  evidence: The resource host resolves and its TLS handshake emits "Request CERT (13)" backed by a private CDR certificate chain - the server demands a client certificate issued by the CDR Register certificate authority. Observed directly; no endpoint behind the gate was called.
  host: https://api.cdr.ergonretail.com.au
  name: CDR mutual TLS (transport)
  type: mutualTLS
- client_authentication: private_key_jwt
  features:
  - Pushed Authorization Requests (PAR)
  - PKCE
  - request object signing (JARM where applicable)
  - CDR Arrangement Revocation endpoint
  - consumer dashboard for consent review and revocation (mandated)
  flows:
  - authorizationUrl: not publicly discoverable
    flow: authorizationCode
    scopes_detail: scopes/energy-queensland-scopes.yml
    tokenUrl: not publicly discoverable
  name: CDR OAuth2 / FAPI 1.0 Advanced
  registration: Dynamic Client Registration using a software statement assertion issued by the CDR Register to an accredited data recipient software product.
  token_binding: mutual-TLS sender-constrained access tokens
  type: oauth2
- evidence: Anonymous OIDC discovery was attempted and refused by design. On 2026-07-27 GET /.well-known/openid-configuration returned HTTP 404 on public.cdr.ergonretail.com.au and on cdr.energymadeeasy.gov.au, and /.well-known/oauth-authorization-server returned 404 on both. A CDR data holder publishes its infosec base URI through the authenticated portion of the CDR Register, so no OIDC metadata document is fetchable without accreditation. See well-known/energy-queensland-well-known.yml.
  name: OpenID Connect
  openIdConnectUrl: not publicly discoverable
  type: openIdConnect
slug: energy-queensland-authentication
source_filename: energy-queensland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  (DSB Consumer Data Standards v1.36.0), plus live probes of Ergon Energy\n  Retail's registered CDR hosts on 2026-07-27.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndescription: >-\n  Energy Queensland's API estate has exactly two authentication postures, and\n  the line between them is statutory rather than commercial. Everything a\n  member of the public can reach is completely unauthenticated - no key, no\n  signup, no terms click-through, only an x-v version header. Everything about\n  an identifiable customer is behind the full Consumer Data Right security\n  profile: ACCC accreditation, mutual TLS with CDR Register-issued certificates,\n  FAPI 1.0 Advanced OAuth2 with private_key_jwt client authentication, OIDC, and\n  per-consumer consent. There is no middle tier, no partner key, no commercial\n\
  \  API deal, and no self-serve credential of any kind.\n  NOTE ON PROVENANCE: the harvested OpenAPI documents declare NO securitySchemes\n  at all (components.securitySchemes is empty in both cds_energy 1.36.0 and\n  cds_common 1.36.0) because the DSB publishes the security model in the\n  Security Profile section of the standard rather than in the swagger. This\n  profile was therefore read from the standard and from live behaviour, not\n  derived by 0-working/derive-authentication.py, which found nothing to derive.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  public_surface_requires_credentials: false\n  gated_surface_requires_accreditation: true\nschemes:\n  - name: none (public CDR surface)\n    type: none\n    applies_to:\n      - listEnergyPlans\n      - getEnergyPlanDetail\n      - getStatus\n      - getOutages\n    hosts:\n      - https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1\n      - https://public.cdr.ergonretail.com.au/cds-au/v1\n\
  \    required_headers:\n      - name: x-v\n        required: true\n        description: >-\n          Requested endpoint version. Mandatory. Omitting it returns HTTP 400\n          urn:au-cds:error:cds-all:Header/Missing - verified live 2026-07-27.\n    optional_headers:\n      - name: x-min-v\n        description: Minimum acceptable endpoint version.\n      - name: x-fapi-interaction-id\n        description: >-\n          RFC 4122 UUID correlation id. Played back verbatim in the response -\n          verified live 2026-07-27 against the AER-hosted plans endpoint.\n    evidence: >-\n      GET https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1/energy/plans with\n      only \"x-v: 1\" returned HTTP 200 with 36 Ergon plans on 2026-07-27, and\n      GET https://public.cdr.ergonretail.com.au/cds-au/v1/discovery/status\n      returned HTTP 200 status OK. No credential of any kind was sent.\n  - name: CDR mutual TLS (transport)\n    type: mutualTLS\n    applies_to: all consumer-authorised energy\
  \ and common operations\n    host: https://api.cdr.ergonretail.com.au\n    evidence: >-\n      The resource host resolves and its TLS handshake emits \"Request CERT (13)\"\n      backed by a private CDR certificate chain - the server demands a client\n      certificate issued by the CDR Register certificate authority. Observed\n      directly; no endpoint behind the gate was called.\n    certificate_authority: CDR Register (ACCC) private CA - transport and signing certificates\n  - name: CDR OAuth2 / FAPI 1.0 Advanced\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: not publicly discoverable\n        tokenUrl: not publicly discoverable\n        scopes_detail: scopes/energy-queensland-scopes.yml\n    client_authentication: private_key_jwt\n    token_binding: mutual-TLS sender-constrained access tokens\n    features:\n      - Pushed Authorization Requests (PAR)\n      - PKCE\n      - request object signing (JARM where applicable)\n      - CDR Arrangement\
  \ Revocation endpoint\n      - consumer dashboard for consent review and revocation (mandated)\n    registration: >-\n      Dynamic Client Registration using a software statement assertion issued by\n      the CDR Register to an accredited data recipient software product.\n  - name: OpenID Connect\n    type: openIdConnect\n    openIdConnectUrl: not publicly discoverable\n    evidence: >-\n      Anonymous OIDC discovery was attempted and refused by design. On\n      2026-07-27 GET /.well-known/openid-configuration returned HTTP 404 on\n      public.cdr.ergonretail.com.au and on cdr.energymadeeasy.gov.au, and\n      /.well-known/oauth-authorization-server returned 404 on both. A CDR data\n      holder publishes its infosec base URI through the authenticated portion of\n      the CDR Register, so no OIDC metadata document is fetchable without\n      accreditation. See well-known/energy-queensland-well-known.yml.\nonboarding:\n  self_serve: false\n  steps:\n    - Apply to the ACCC for accreditation\
  \ as a CDR data recipient (unrestricted or sponsored), or operate under the CDR representative / trusted adviser pathways.\n    - Obtain client credentials plus transport and signing certificates from the CDR Register certificate authority.\n    - Complete Conformance Test Suite (CTS) testing.\n    - Register the software product and complete Dynamic Client Registration with the data holder.\n    - Initiate a consent flow that the individual Ergon Energy Retail customer approves.\n  gate: statutory, not commercial\nrelated:\n  scopes: scopes/energy-queensland-scopes.yml\n  conventions: conventions/energy-queensland-conventions.yml\n  conformance: conformance/energy-queensland-conformance.yml\n  well_known: well-known/energy-queensland-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/authentication/energy-queensland-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Queensland
- Smart Metering
- Solar
- DER
- Open Data
---
