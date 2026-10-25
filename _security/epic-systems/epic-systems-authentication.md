---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Epic Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epic Systems declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Epic Systems
provider_slug: epic-systems
scheme_count: 3
schemes:
- authorizationUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  name: SMART-on-FHIR-OAuth2
  tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token
  type: oauth2
- issuer: https://fhir.epic.com/interconnect-fhir-oauth/oauth2
  name: OpenID Connect
  type: openIdConnect
- name: Basic
  note: Listed in the CapabilityStatement security.service codes.
  scheme: basic
  type: http
slug: epic-systems-authentication
source_filename: epic-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: fhir/epic-fhir-r4-smart-configuration.json\ndocs: https://fhir.epic.com/Documentation?docId=oauth2\nschemes:\n- name: SMART-on-FHIR-OAuth2\n  type: oauth2\n  authorizationUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n  tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\n  grant_types: &id001\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n- name: OpenID Connect\n  type: openIdConnect\n  issuer: https://fhir.epic.com/interconnect-fhir-oauth/oauth2\n- name: Basic\n  type: http\n  scheme: basic\n  note: Listed in the CapabilityStatement security.service codes.\naid: epic-systems\nname: Epic Systems Authentication\nprovider: Epic on FHIR\ndate: '2026-07-24'\nreviewer: API Evangelist\nsummary: Epic's FHIR APIs are authorized with SMART on FHIR / OAuth 2.0. The live R4\
  \ .well-known/smart-configuration\n  was fetched anonymously and captured verbatim at fhir/epic-fhir-r4-smart-configuration.json. Two SMART\n  app launch flows are supported (EHR launch and standalone launch), plus a backend-services client-credentials\n  flow using asymmetric (JWT) client authentication for system-level and Bulk Data access.\nmodel: SMART on FHIR / OAuth 2.0\nwellKnown:\n  smartConfiguration: https://fhir.epic.com/interconnect-fhir-oauth/api/FHIR/R4/.well-known/smart-configuration\n  status: 200\n  capturedFile: fhir/epic-fhir-r4-smart-configuration.json\nendpoints:\n  issuer: https://fhir.epic.com/interconnect-fhir-oauth/oauth2\n  authorization: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n  token: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\ngrantTypesSupported: *id001\nsmartCapabilities:\n- launch-ehr\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- client-confidential-asymmetric\n- context-banner\n- context-style\n\
  - context-ehr-patient\n- context-ehr-encounter\n- context-standalone-patient\n- permission-offline\n- permission-patient\n- permission-user\n- permission-v1\n- permission-v2\n- sso-openid-connect\n- authorize-post\nscopeModel:\n  note: Epic uses SMART on FHIR scope grammar. The smart-configuration advertises base scopes (openid,\n    profile, fhirUser, launch). Resource access is granted with SMART v1/v2 scopes of the form patient/<Resource>.<read|search|...>,\n    user/<Resource>.<...>, and system/<Resource>.<...> negotiated per registered client and health-system\n    authorization; both permission-v1 and permission-v2 scope styles are supported.\n  advertisedScopes:\n  - epic.scanning.dmsusername\n  - fhirUser\n  - launch\n  - openid\n  - profile\ncapabilityStatementSecurity:\n  service:\n  - OAuth\n  - SMART-on-FHIR\n  - Basic\n  oauthUris:\n    authorize: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n    token: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\n\
  gating: The sandbox is openly reachable for testing; production access requires app registration on the\n  Epic on FHIR developer portal plus a connected health system's activation of the app.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-systems/refs/heads/main/authentication/epic-systems-authentication.yml
summary_line: 3 schemes
tags:
- Healthcare
- United States
- Electronic Health Records
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- US Core
- Clinical Data
---
