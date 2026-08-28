---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Octagos Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octagos Health declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Octagos Health
provider_slug: octagos-health
scheme_count: 4
schemes:
- audience: clinic and health-system staff
  evidence: '"Multi-factor authentication and SAML 2.0 single sign-on" (octagos.com/solutions/it).'
  id: saml2-sso
  type: saml2
- audience: Epic end users
  evidence: '"Direct deployment of Octagos from Epic with SSO + MFA" (octagos.com/solutions/it); "Epic single sign-on (SSO) and multi-factor authentication (MFA)" (octagos.com/solutions/ehr/epic).'
  id: epic-sso
  type: sso
- audience: Oracle Health end users
  evidence: '"single sign-on (SSO) and multi-factor authentication (MFA) streamline access while reducing risk" (octagos.com/solutions/ehr/oracle-health).'
  id: oracle-health-sso
  type: sso
- audience: the EHR's FHIR authorization server, not Octagos
  direction: outbound
  evidence: '"Epic Showroom-listed for SMART on FHIR" (octagos.com/solutions/ehr/epic). The SMART App Launch framework requires an OAuth 2.0 authorization-code exchange, but the authorization server belongs to the customer''s EHR. Octagos publishes no scope list, no launch context documentation and no redirect-URI registration guidance, so this cannot be exercised from the public surface.'
  flow: authorization_code
  id: smart-on-fhir-oauth2
  type: oauth2
slug: octagos-health-authentication
source_filename: octagos-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://www.octagos.com/solutions/it, https://www.octagos.com/solutions/ehr/epic,\n  https://www.octagos.com/solutions/ehr/oracle-health, plus direct probes of\n  app.octagos.com — 2026-08-26.\nnote: >-\n  DERIVED FROM DOCS ONLY. Octagos publishes no OpenAPI, so there are no securitySchemes\n  to read. Everything below describes how humans and EHR systems authenticate INTO the\n  Octagos application, not how a developer would authenticate against a public API —\n  because no public API is offered. There is no published API-key issuance flow, no\n  token endpoint, and no developer credential of any kind.\npublic_api_authentication:\n  available: false\n  evidence: >-\n    No developer portal, no API reference, no signup that yields a credential. The only\n    credentialed surface reachable from the public internet is the tenant application at\n    https://app.octagos.com (HTTP 200, Angular SPA login), whose backend answers\n\
  \    /api/health with HTTP 503 \"Unhealthy\" — proving a real API router exists behind the\n    login, but nothing about it is documented.\nschemes:\n- id: saml2-sso\n  type: saml2\n  audience: clinic and health-system staff\n  evidence: '\"Multi-factor authentication and SAML 2.0 single sign-on\" (octagos.com/solutions/it).'\n- id: epic-sso\n  type: sso\n  audience: Epic end users\n  evidence: >-\n    \"Direct deployment of Octagos from Epic with SSO + MFA\" (octagos.com/solutions/it);\n    \"Epic single sign-on (SSO) and multi-factor authentication (MFA)\"\n    (octagos.com/solutions/ehr/epic).\n- id: oracle-health-sso\n  type: sso\n  audience: Oracle Health end users\n  evidence: >-\n    \"single sign-on (SSO) and multi-factor authentication (MFA) streamline access while\n    reducing risk\" (octagos.com/solutions/ehr/oracle-health).\n- id: smart-on-fhir-oauth2\n  type: oauth2\n  flow: authorization_code\n  direction: outbound\n  audience: the EHR's FHIR authorization server, not Octagos\n\
  \  evidence: >-\n    \"Epic Showroom-listed for SMART on FHIR\" (octagos.com/solutions/ehr/epic). The\n    SMART App Launch framework requires an OAuth 2.0 authorization-code exchange, but the\n    authorization server belongs to the customer's EHR. Octagos publishes no scope list,\n    no launch context documentation and no redirect-URI registration guidance, so this\n    cannot be exercised from the public surface.\nmfa:\n  required: true\n  evidence: MFA is stated alongside SSO on the IT, Epic and Oracle Health pages.\ndiscovery_probes:\n- url: https://app.octagos.com/.well-known/openid-configuration\n  status: 404\n- url: https://app.octagos.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://app.octagos.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://www.octagos.com/.well-known/openid-configuration\n  status: 404\nscopes_artifact: >-\n  Not written. scopes/ is OAuth-only and requires a scope reference to derive from;\n  Octagos documents\
  \ no scopes of its own (the SMART on FHIR scopes in play belong to the\n  customer's EHR). Forcing an empty scopes artifact would misrepresent the surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octagos-health/refs/heads/main/authentication/octagos-health-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Healthcare
- Cardiology
- Remote Patient Monitoring
- Medical Devices
- Artificial Intelligence
- Health IT
- Interoperability
- FHIR
- EHR Integration
- Clinical Workflow
---
