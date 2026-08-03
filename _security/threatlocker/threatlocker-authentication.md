---
api_key_in:
- header
api_specs:
- filename: threatlocker-portal-openapi-original.json
  format: json
  label: ThreatLocker PortalAPI
  slug: threatlocker-portalapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-portal-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Threatlocker Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThreatLocker secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ThreatLocker
provider_slug: threatlocker
scheme_count: 3
schemes:
- authorization: Roles and the organizations the token is valid for are selected at creation time.
  description: Please insert Standard Authorization header.
  docs_description: API User token created in the ThreatLocker Portal under Users > API Users > New API User > Generate API Token. Sent verbatim in the Authorization header with an auth type of "API Key" — there is NO Bearer prefix. The token is displayed only once, while the creation sidebar is open.
  expiry: Inactivity-based. The selected expiration window (e.g. 90 days) RESETS on every use, so the token expires only after that period of inactivity.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/threatlocker-portal-openapi-original.json
  - https://threatlocker.kb.help/api-users/
  type: apiKey
- description: Please insert Managed Organization Id.
  docs_description: Documented in the Getting Started guide as a header named "managedOrganizationId" carrying the target organization's GUID, copied from Manage > Organizations > (settings) > Organization ID. Selects the tenant a request acts against; required when a parent (MSP) token operates on a managed child organization.
  in: header
  name: ManagedOrganizationId
  parameter: ManagedOrganizationId
  sources:
  - openapi/threatlocker-portal-openapi-original.json
  - https://threatlocker.kb.help/getting-started-with-threatlocker-portalapis/
  type: apiKey
- description: Please insert Managed Organization Id.
  docs_description: Third apiKey scheme declared in the spec for overriding the managed-organization scope of a request.
  in: header
  name: OverrideManagedOrganizationId
  parameter: OverrideManagedOrganizationId
  sources:
  - openapi/threatlocker-portal-openapi-original.json
  type: apiKey
slug: threatlocker-authentication
source_filename: threatlocker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/threatlocker-portal-openapi-original.json\ndocs: https://threatlocker.kb.help/api-users/\ndocs_getting_started: https://threatlocker.kb.help/getting-started-with-threatlocker-portalapis/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The PortalAPI is API-key only. There is no OAuth 2.0, no OIDC discovery document, and no scope\n    surface — authorization is expressed as ROLES bound to the token at creation time, plus an\n    organization scope, neither of which is exposed in the OpenAPI. Portal ADMINISTRATOR sign-in is a\n    separate concern and does support SAML SSO and SCIM provisioning; those do not apply to API tokens.\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Please insert Standard Authorization header.\n  docs_description: >-\n    API User token created in the ThreatLocker Portal under Users > API\
  \ Users > New API User >\n    Generate API Token. Sent verbatim in the Authorization header with an auth type of \"API Key\" —\n    there is NO Bearer prefix. The token is displayed only once, while the creation sidebar is open.\n  expiry: >-\n    Inactivity-based. The selected expiration window (e.g. 90 days) RESETS on every use, so the token\n    expires only after that period of inactivity.\n  authorization: Roles and the organizations the token is valid for are selected at creation time.\n  sources:\n  - openapi/threatlocker-portal-openapi-original.json\n  - https://threatlocker.kb.help/api-users/\n- name: ManagedOrganizationId\n  type: apiKey\n  in: header\n  parameter: ManagedOrganizationId\n  description: Please insert Managed Organization Id.\n  docs_description: >-\n    Documented in the Getting Started guide as a header named \"managedOrganizationId\" carrying the\n    target organization's GUID, copied from Manage > Organizations > (settings) > Organization ID.\n    Selects\
  \ the tenant a request acts against; required when a parent (MSP) token operates on a\n    managed child organization.\n  sources:\n  - openapi/threatlocker-portal-openapi-original.json\n  - https://threatlocker.kb.help/getting-started-with-threatlocker-portalapis/\n- name: OverrideManagedOrganizationId\n  type: apiKey\n  in: header\n  parameter: OverrideManagedOrganizationId\n  description: Please insert Managed Organization Id.\n  docs_description: Third apiKey scheme declared in the spec for overriding the managed-organization scope of a request.\n  sources:\n  - openapi/threatlocker-portal-openapi-original.json\nglobal_security:\n  note: All three schemes are listed in the document-level `security` requirement of the OpenAPI.\n  requirement: [Authorization, ManagedOrganizationId, OverrideManagedOrganizationId]\nportal_administrator_sign_in:\n  note: Separate from API tokens — governs human sign-in to the ThreatLocker Portal, not PortalAPI calls.\n  saml_sso: true\n  saml_docs: https://threatlocker.kb.help/saml-integration/\n\
  \  saml_detail: Enabled via Administrators > Login Settings > Allow SSO; IdP groups map to ThreatLocker user roles on the Group Mapping tab.\n  scim: true\n  scim_docs: https://threatlocker.kb.help/scim-integration-for-threatlocker-administrator-accounts/\n  scim_detail: SCIM provisioning of administrators available since Portal 3.8; provisioned users get a SAML-enabled account or an email invitation.\n  oidc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/authentication/threatlocker-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- cybersecurity
- zero-trust
- endpoint-security
- application-control
- allowlisting
- ransomware-prevention
- privileged-access-management
- network-access-control
- managed-detection-and-response
- device-management
- msp
- compliance
---
