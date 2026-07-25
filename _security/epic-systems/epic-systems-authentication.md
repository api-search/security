---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: ''
name: Epic Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epic Systems declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Epic Systems
provider_slug: epic-systems
scheme_count: 0
schemes: []
slug: epic-systems-authentication
source_filename: epic-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "aid: epic-systems\nname: Epic Systems Authentication\nprovider: Epic on FHIR\ndate: '2026-07-24'\nreviewer: API Evangelist\nsummary: >-\n  Epic's FHIR APIs are authorized with SMART on FHIR / OAuth 2.0. The live\n  R4 .well-known/smart-configuration was fetched anonymously and captured\n  verbatim at fhir/epic-fhir-r4-smart-configuration.json. Two SMART app\n  launch flows are supported (EHR launch and standalone launch), plus a\n  backend-services client-credentials flow using asymmetric (JWT) client\n  authentication for system-level and Bulk Data access.\nmodel: SMART on FHIR / OAuth 2.0\nwellKnown:\n  smartConfiguration: https://fhir.epic.com/interconnect-fhir-oauth/api/FHIR/R4/.well-known/smart-configuration\n  status: 200\n  capturedFile: fhir/epic-fhir-r4-smart-configuration.json\nendpoints:\n  issuer: https://fhir.epic.com/interconnect-fhir-oauth/oauth2\n  authorization: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n  token: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\n\
  grantTypesSupported:\n- authorization_code\n- refresh_token\n- client_credentials\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:ietf:params:oauth:grant-type:token-exchange\nsmartCapabilities:\n- launch-ehr\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- client-confidential-asymmetric\n- context-banner\n- context-style\n- context-ehr-patient\n- context-ehr-encounter\n- context-standalone-patient\n- permission-offline\n- permission-patient\n- permission-user\n- permission-v1\n- permission-v2\n- sso-openid-connect\n- authorize-post\nscopeModel:\n  note: >-\n    Epic uses SMART on FHIR scope grammar. The smart-configuration advertises\n    base scopes (openid, profile, fhirUser, launch). Resource access is granted\n    with SMART v1/v2 scopes of the form patient/<Resource>.<read|search|...>,\n    user/<Resource>.<...>, and system/<Resource>.<...> negotiated per registered\n    client and health-system authorization; both permission-v1 and permission-v2\n \
  \   scope styles are supported.\n  advertisedScopes:\n  - epic.scanning.dmsusername\n  - fhirUser\n  - launch\n  - openid\n  - profile\ncapabilityStatementSecurity:\n  service:\n  - OAuth\n  - SMART-on-FHIR\n  - Basic\n  oauthUris:\n    authorize: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n    token: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\ngating: >-\n  The sandbox is openly reachable for testing; production access requires app\n  registration on the Epic on FHIR developer portal plus a connected health\n  system's activation of the app.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-systems/refs/heads/main/authentication/epic-systems-authentication.yml
summary_line: 0 schemes
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- US Core
- Clinical Data
---
