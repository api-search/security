---
api_key_in: []
auth_types:
- mutualTLS
- nhs-jwt
- approval-gated-socket
description: ''
kind: authentication
layout: security
method: searched
name: Tpp Systmone Authentication
name_suffix: Authentication
oauth_flows: []
overview: TPP (SystmOne) secures its APIs with mutualTLS, nhs-jwt, and approval-gated-socket across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TPP (SystmOne)
provider_slug: tpp-systmone
scheme_count: 3
schemes:
- api: SystmOne Client Integration API
  description: An approved third-party application interacts with a running SystmOne client over a local TCP socket, exchanging XML documents validated against published XSD schemas. There is no bearer token or OAuth flow; access is gated by TPP's Integration Request approval and organisation-level enablement rather than a runtime credential handshake.
  name: SystmOneClientIntegrationApproval
  source: https://tpp-uk.com/resources/integration-request/
  transport: XML over local TCP socket
  type: approval-gated
- api: Interface Mechanism 1 (IM1)
  description: IM1 Transaction, Bulk, and Patient Facing Services integrations are onboarded through the NHS England Digital Care Services IM1 Pairing Integration Process and a Supplier Conformance Assessment List (SCAL). Endpoints are provisioned per approved pairing; credentials and connection details are issued as part of conformance, not self-serve.
  name: IM1PairingConformance
  source: https://digital.nhs.uk/developer/api-catalogue/interface-mechanism-1-standards
  type: nhs-conformance
- api: GP Connect (FHIR)
  description: GP Connect FHIR requests are routed through the NHS Spine Secure Proxy (SSP), a forward HTTP proxy that is the single point of authentication and authorisation. Each request carries an NHS-issued JSON Web Token (JWT) conveying cross-organisation audit and provenance (issuer, requesting system, requesting organisation, requesting user); insufficient audit information causes the SSP to block the request. Both legs of the request (consumer-to-proxy and proxy-to-provider) are secured with mutual TLS.
  mechanisms:
  - json_web_token: NHS cross-organisation audit and provenance JWT
  - mutual_tls: TLS-MA on both request legs via Spine Secure Proxy
  - data_sharing_agreement_check: enforced by SSP
  name: GPConnectSpineSecureProxyJWT
  source: https://nhsconnect.github.io/FHIR-SpineCore/ssp_overview.html
  type: nhs-jwt
slug: tpp-systmone-authentication
source_filename: tpp-systmone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  https://digital.nhs.uk/services/gp-connect ,\n  https://nhsconnect.github.io/FHIR-SpineCore/ssp_overview.html ,\n  https://tpp-uk.com/resources/integration-request/\nnote: >-\n  TPP SystmOne publishes no OpenAPI and no public OAuth surface; authentication cannot be\n  derived from a spec. This profile is searched from TPP's Integration Request materials\n  and the NHS England GP Connect / IM1 / Spine Secure Proxy documentation. Three distinct\n  auth models apply depending on the integration route.\nsummary:\n  types: [mutualTLS, nhs-jwt, approval-gated-socket]\n  public_self_serve: false\n  onboarding: NHS partner conformance (Integration Request / IM1 Pairing / SCAL)\nschemes:\n  - name: SystmOneClientIntegrationApproval\n    api: SystmOne Client Integration API\n    type: approval-gated\n    transport: XML over local TCP socket\n    description: >-\n      An approved third-party application interacts with a running\
  \ SystmOne client over a\n      local TCP socket, exchanging XML documents validated against published XSD schemas.\n      There is no bearer token or OAuth flow; access is gated by TPP's Integration Request\n      approval and organisation-level enablement rather than a runtime credential handshake.\n    source: https://tpp-uk.com/resources/integration-request/\n  - name: IM1PairingConformance\n    api: Interface Mechanism 1 (IM1)\n    type: nhs-conformance\n    description: >-\n      IM1 Transaction, Bulk, and Patient Facing Services integrations are onboarded through\n      the NHS England Digital Care Services IM1 Pairing Integration Process and a Supplier\n      Conformance Assessment List (SCAL). Endpoints are provisioned per approved pairing;\n      credentials and connection details are issued as part of conformance, not self-serve.\n    source: https://digital.nhs.uk/developer/api-catalogue/interface-mechanism-1-standards\n  - name: GPConnectSpineSecureProxyJWT\n    api: GP Connect\
  \ (FHIR)\n    type: nhs-jwt\n    description: >-\n      GP Connect FHIR requests are routed through the NHS Spine Secure Proxy (SSP), a\n      forward HTTP proxy that is the single point of authentication and authorisation.\n      Each request carries an NHS-issued JSON Web Token (JWT) conveying cross-organisation\n      audit and provenance (issuer, requesting system, requesting organisation, requesting\n      user); insufficient audit information causes the SSP to block the request. Both legs\n      of the request (consumer-to-proxy and proxy-to-provider) are secured with mutual TLS.\n    mechanisms:\n      - json_web_token: NHS cross-organisation audit and provenance JWT\n      - mutual_tls: TLS-MA on both request legs via Spine Secure Proxy\n      - data_sharing_agreement_check: enforced by SSP\n    source: https://nhsconnect.github.io/FHIR-SpineCore/ssp_overview.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpp-systmone/refs/heads/main/authentication/tpp-systmone-authentication.yml
summary_line: mutualTLS/nhs-jwt/approval-gated-socket · 3 schemes
tags:
- Healthcare
- United Kingdom
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- GP Connect
- IM1
- National Health System
- Primary Care
- Clinical System
---
