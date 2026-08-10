---
api_key_in: []
auth_types:
- saml
- ldap
- password
- mfa
- biometric
description: ''
kind: authentication
layout: security
method: searched
name: Exo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exo secures its APIs with saml, ldap, password, mfa, and biometric across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Exo
provider_slug: exo
scheme_count: 5
schemes:
- evidence: '"Single Sign On (SSO) with SAML"'
  name: SAML single sign-on
  source: https://www.exo.inc/exo-works/specs
  tier: Exo Works Connect and Enterprise
  type: saml2
- evidence: '"Active Directory (LDAP)*" (* requires Exo Works Enterprise)'
  name: Active Directory (LDAP)
  source: https://www.exo.inc/exo-works/specs
  tier: Exo Works Enterprise
  type: ldap
- evidence: registration and first-time sign-in flow documented in the support portal
  name: Username and password
  source: https://support.exo.inc/hc/en-us/sections/22799151240603-Sign-In
  type: password
- evidence: multi-factor authentication listed among Exo Iris device access controls
  name: Multi-factor authentication
  source: https://www.exo.inc/iris/integrations
  type: mfa
- evidence: Face ID, Touch ID and PIN code listed as Exo Iris access controls
  name: Device biometrics / PIN
  source: https://www.exo.inc/iris/integrations
  type: biometric
slug: exo-authentication
source_filename: exo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://www.exo.inc/exo-works/specs\ndocs:\n- https://www.exo.inc/exo-works/specs\n- https://support.exo.inc/hc/en-us/sections/22799151240603-Sign-In\n- https://www.exo.inc/iris/integrations\nscope: platform\nscope_note: 'This is the authentication model Exo documents for its Exo Works platform\n  and Exo Iris mobile application. Exo publishes no public developer API and therefore\n  no API authentication scheme, no API keys, no OAuth surface and no securitySchemes\n  to derive from. Nothing here was derived from a specification.'\nsummary:\n  types:\n  - saml\n  - ldap\n  - password\n  - mfa\n  - biometric\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: SAML single sign-on\n  type: saml2\n  tier: Exo Works Connect and Enterprise\n  evidence: '\"Single Sign On (SSO) with SAML\"'\n  source: https://www.exo.inc/exo-works/specs\n- name: Active Directory (LDAP)\n  type: ldap\n  tier: Exo Works Enterprise\n  evidence: '\"\
  Active Directory (LDAP)*\" (* requires Exo Works Enterprise)'\n  source: https://www.exo.inc/exo-works/specs\n- name: Username and password\n  type: password\n  evidence: registration and first-time sign-in flow documented in the support portal\n  source: https://support.exo.inc/hc/en-us/sections/22799151240603-Sign-In\n- name: Multi-factor authentication\n  type: mfa\n  evidence: multi-factor authentication listed among Exo Iris device access controls\n  source: https://www.exo.inc/iris/integrations\n- name: Device biometrics / PIN\n  type: biometric\n  evidence: Face ID, Touch ID and PIN code listed as Exo Iris access controls\n  source: https://www.exo.inc/iris/integrations\nsession:\n  web_idle_timeout_minutes: 15\n  auto_log_off: true\n  single_device: 'mobile sessions terminate when the same user signs in on another\n    device (USER_SESSION_TIMEOUT event)'\n  source: https://support.exo.inc/hc/en-us/articles/50040102231707-Iris-Activity-Events-Export-Available-Fields\nauthorization:\n\
  \  model: role-based access control (RBAC)\n  evidence: '\"Role-based access control (RBAC)\" under Access'\n  source: https://www.exo.inc/exo-works/specs\ngaps:\n- No public API authentication documentation - Exo publishes no developer API.\n- api.prod.exoworks.inc (AWS API Gateway) rejects anonymous requests with HTTP 403\n  and publishes no authentication guidance.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on\n  any Exo host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exo/refs/heads/main/authentication/exo-authentication.yml
summary_line: saml/ldap/password/mfa/biometric · 5 schemes
tags:
- Company
- Health
- Healthcare
- Medical Imaging
- Ultrasound
- Point of Care
- Artificial Intelligence
- Medical Devices
- DICOM
- HL7
---
