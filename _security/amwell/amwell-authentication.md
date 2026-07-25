---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Amwell Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Amwell secures its APIs with oauth2, openIdConnect, and saml across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Amwell
provider_slug: amwell
scheme_count: 4
schemes:
- evidence: keycloak.dev.americanwell.com referenced in developers.amwell.com CSP
  name: oidc
  provider: Keycloak
  scheme: openid-connect
  type: openIdConnect
- evidence: Keycloak OAuth 2.0 authorization endpoint for platform/API access
  flows:
  - authorizationCode
  name: oauth2
  type: oauth2
- evidence: Single sign-on for EHR (Epic, Oracle Cerner) and patient-portal launch of embedded virtual visits, per Amwell Converge platform documentation.
  name: saml-sso
  scheme: single-sign-on
  type: saml
- evidence: FHIR-based EHR launch workflows over SSO
  name: smart-on-fhir
  scheme: smart-on-fhir
  type: oauth2
slug: amwell-authentication
source_filename: amwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  Content-Security-Policy of developers.amwell.com (Keycloak IdP) +\n  Amwell Converge platform single-sign-on documentation\nnote: >-\n  The Amwell Converge REST/FHIR API reference sits behind the gated partner\n  developer portal (developers.amwell.com), so no OpenAPI securitySchemes could\n  be derived mechanically. This profile is assembled from Amwell's public\n  single-sign-on statements and the identity infrastructure exposed in the\n  developer/telehealth client's Content-Security-Policy.\nsummary:\n  types: [oauth2, openIdConnect, saml]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  identity_provider: Keycloak (keycloak.dev.americanwell.com)\nschemes:\n  - name: oidc\n    type: openIdConnect\n    scheme: openid-connect\n    provider: Keycloak\n    evidence: keycloak.dev.americanwell.com referenced in developers.amwell.com CSP\n  - name: oauth2\n    type: oauth2\n    flows: [authorizationCode]\n    evidence:\
  \ Keycloak OAuth 2.0 authorization endpoint for platform/API access\n  - name: saml-sso\n    type: saml\n    scheme: single-sign-on\n    evidence: >-\n      Single sign-on for EHR (Epic, Oracle Cerner) and patient-portal launch of\n      embedded virtual visits, per Amwell Converge platform documentation.\n  - name: smart-on-fhir\n    type: oauth2\n    scheme: smart-on-fhir\n    evidence: FHIR-based EHR launch workflows over SSO\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amwell/refs/heads/main/authentication/amwell-authentication.yml
summary_line: oauth2/openIdConnect/saml · 4 schemes
tags:
- Healthcare
- United States
- Telehealth
- Virtual Care
- FHIR
- HL7
- Interoperability
- EHR
- SDK
---
