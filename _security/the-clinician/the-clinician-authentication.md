---
api_key_in: []
auth_types: []
description: 'Authentication and access-control profile for The Clinician Platform (TCP), read from the enterprise capabilities and integration sections of the company''s own homepage. THIS IS NOT DERIVED FROM A CONTRACT: The Clinician publishes no OpenAPI, so there are no securitySchemes to read and no token endpoint, header name, scope string or grant type is public. What follows is the authentication MODEL the provider describes in prose, recorded so an integrator knows what to expect before the sales conversation — not a specification an agent can act on.'
kind: authentication
layout: security
method: searched
name: The Clinician Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Clinician declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: The Clinician
provider_slug: the-clinician
scheme_count: 4
schemes:
- detail: '"Integrates with your organisation''s Active Directory to mirror existing roles and permissions." The integration diagram names an IDENTITY lane of Active Directory / SAML / OAuth / SCIM, and the integration capability summarises as "FHIR-native · HL7 · REST APIs · SSO/SAML".'
  documented: true
  id: enterprise-sso
  source: https://theclinician.com/
  type: federated
- detail: The provider states organisations can "extend [AD roles] with TCP-specific scopes where the platform needs finer-grained control". No scope reference, naming convention or authorization server is published, so no scopes/ artifact is written — an empty or invented scope list would be worse than the honest gap.
  documented: partial
  id: tcp-scopes
  source: https://theclinician.com/
  type: oauth2-like
- detail: '"EHR iframe embedding via signed tokens" — the mechanism by which TCP is surfaced inside a host EHR session. Token format, signing algorithm, claim set and lifetime are all unpublished.'
  documented: true
  id: signed-token-embed
  source: https://theclinician.com/
  type: signed-token
- detail: Two-factor authentication is stated as available for platform users.
  documented: true
  id: mfa
  source: https://theclinician.com/
  type: second-factor
slug: the-clinician-authentication
source_filename: the-clinician-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://theclinician.com/\ndocs: https://theclinician.com/\ndescription: >-\n  Authentication and access-control profile for The Clinician Platform (TCP),\n  read from the enterprise capabilities and integration sections of the company's\n  own homepage. THIS IS NOT DERIVED FROM A CONTRACT: The Clinician publishes no\n  OpenAPI, so there are no securitySchemes to read and no token endpoint, header\n  name, scope string or grant type is public. What follows is the authentication\n  MODEL the provider describes in prose, recorded so an integrator knows what to\n  expect before the sales conversation — not a specification an agent can act on.\nschemes:\n  - id: enterprise-sso\n    type: federated\n    documented: true\n    detail: >-\n      \"Integrates with your organisation's Active Directory to mirror existing\n      roles and permissions.\" The integration diagram names an IDENTITY lane of\n      Active Directory / SAML /\
  \ OAuth / SCIM, and the integration capability\n      summarises as \"FHIR-native · HL7 · REST APIs · SSO/SAML\".\n    source: https://theclinician.com/\n  - id: tcp-scopes\n    type: oauth2-like\n    documented: partial\n    detail: >-\n      The provider states organisations can \"extend [AD roles] with TCP-specific\n      scopes where the platform needs finer-grained control\". No scope reference,\n      naming convention or authorization server is published, so no scopes/\n      artifact is written — an empty or invented scope list would be worse than\n      the honest gap.\n    source: https://theclinician.com/\n  - id: signed-token-embed\n    type: signed-token\n    documented: true\n    detail: >-\n      \"EHR iframe embedding via signed tokens\" — the mechanism by which TCP is\n      surfaced inside a host EHR session. Token format, signing algorithm, claim\n      set and lifetime are all unpublished.\n    source: https://theclinician.com/\n  - id: mfa\n    type: second-factor\n\
  \    documented: true\n    detail: Two-factor authentication is stated as available for platform users.\n    source: https://theclinician.com/\nauthorization_model:\n  style: group-and-role-based, within a per-deployment organisational hierarchy\n  tenancy: >-\n    \"Multi-tenant isolation enforced at the API boundary on every request\" —\n    the only statement the company makes about its API boundary behaviour.\n  data_minimisation: >-\n    PII can be restricted per health service: clinical teams see their own\n    patients identifiably, cross-organisational users see aggregated, anonymised\n    data only.\n  audit: Full audit trail across authentication, authorisation and data access.\n  source: https://theclinician.com/\ndiscovery_probes:\n  - url: https://theclinician.com/.well-known/openid-configuration\n    status: 404\n  - url: https://theclinician.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://theclinician.com/.well-known/oauth-protected-resource\n\
  \    status: 404\ngaps:\n  - No public token endpoint, grant type, header name or key format.\n  - No authorization-server or protected-resource metadata at any well-known path.\n  - >-\n    No public scope reference, so the \"TCP-specific scopes\" the provider markets\n    cannot be evaluated by a buyer or consumed by an agent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-clinician/refs/heads/main/authentication/the-clinician-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Healthcare
- Health IT
- Patient Reported Outcomes
- PROMs
- Value-Based Care
- Clinical Data
- Interoperability
- FHIR
- openEHR
- Digital Health
- New Zealand
---
