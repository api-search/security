---
api_key_in: []
auth_types:
- mutualTLS
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Australian Digital Health Agency Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Digital Health Agency secures its APIs with mutualTLS, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australian Digital Health Agency
provider_slug: australian-digital-health-agency
scheme_count: 3
schemes:
- applies_to:
  - My Health Record FHIR Gateway (B2B)
  - My Health Record FHIR Mobile Gateway
  - Healthcare Identifiers (HI) Service
  - Electronic Prescribing
  description: Connections to the national record systems are authenticated with a National Authentication Service for Health (NASH) SHA-2 PKI certificate presented over mutual TLS. NASH certificates are issued to conformant, registered healthcare organisations (identified by an HPI-O) after onboarding and conformance testing.
  docs: https://implementer.digitalhealth.gov.au/resources/services/national-authentication-service-for-health-nash
  issuance: Gated — registration + conformance + NASH certificate issuance (Services Australia).
  name: NASH-PKI-mTLS
  type: mutualTLS
- applies_to:
  - NCTS FHIR Terminology Server
  cors: true
  flows:
  - authorizationUrl: https://api.healthterminologies.gov.au/oauth2/login
    flow: authorizationCode
    scopes:
      openid: OpenID Connect authentication
      profile: Basic profile claims
    tokenUrl: https://api.healthterminologies.gov.au/oauth2/token
  name: SMART-on-FHIR-OAuth2
  profile: SMART-on-FHIR (http://docs.smarthealthit.org)
  sources:
  - fhir/ncts-terminology-server-capabilitystatement.json
  - well-known/australian-digital-health-agency-smart-configuration.json
  type: oauth2
- applies_to:
  - NCTS FHIR Terminology Server
  description: The NCTS terminology server advertises the openid scope alongside SMART-on-FHIR OAuth2.
  name: OpenIDConnect
  type: openIdConnect
slug: australian-digital-health-agency-authentication
source_filename: australian-digital-health-agency-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  fhir/ncts-terminology-server-capabilitystatement.json (CapabilityStatement.rest.security),\n  well-known/australian-digital-health-agency-smart-configuration.json,\n  https://implementer.digitalhealth.gov.au/resources/services/national-authentication-service-for-health-nash\nsummary:\n  types: [mutualTLS, oauth2, openIdConnect]\n  models:\n    - national-record-systems: NASH SHA-2 PKI client certificate over mutual TLS\n    - terminology-server: SMART-on-FHIR OAuth2 (authorization code) + OpenID Connect\nschemes:\n  - name: NASH-PKI-mTLS\n    type: mutualTLS\n    applies_to:\n      - My Health Record FHIR Gateway (B2B)\n      - My Health Record FHIR Mobile Gateway\n      - Healthcare Identifiers (HI) Service\n      - Electronic Prescribing\n    description: >-\n      Connections to the national record systems are authenticated with a National\n      Authentication Service for Health (NASH) SHA-2 PKI certificate presented\
  \ over\n      mutual TLS. NASH certificates are issued to conformant, registered healthcare\n      organisations (identified by an HPI-O) after onboarding and conformance testing.\n    issuance: Gated — registration + conformance + NASH certificate issuance (Services Australia).\n    docs: https://implementer.digitalhealth.gov.au/resources/services/national-authentication-service-for-health-nash\n  - name: SMART-on-FHIR-OAuth2\n    type: oauth2\n    applies_to:\n      - NCTS FHIR Terminology Server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.healthterminologies.gov.au/oauth2/login\n        tokenUrl: https://api.healthterminologies.gov.au/oauth2/token\n        scopes:\n          openid: OpenID Connect authentication\n          profile: Basic profile claims\n    profile: SMART-on-FHIR (http://docs.smarthealthit.org)\n    cors: true\n    sources:\n      - fhir/ncts-terminology-server-capabilitystatement.json\n      - well-known/australian-digital-health-agency-smart-configuration.json\n\
  \  - name: OpenIDConnect\n    type: openIdConnect\n    applies_to:\n      - NCTS FHIR Terminology Server\n    description: The NCTS terminology server advertises the openid scope alongside SMART-on-FHIR OAuth2.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-digital-health-agency/refs/heads/main/authentication/australian-digital-health-agency-authentication.yml
summary_line: mutualTLS/oauth2/openIdConnect · 3 schemes
tags:
- Healthcare
- Australia
- National Health System
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Electronic Health Record
- e-Prescribing
- Terminology
- Government
---
