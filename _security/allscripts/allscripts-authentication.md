---
api_key_in: []
auth_types: []
description: Authentication profile for the Veradigm FHIR R4 API. The API supports SMART on FHIR (HL7 SMART App Launch) OAuth 2.0. Veradigm's own docs describe three distinct authentication paths, and the live smart-configuration document confirms three OAuth grant types and both public and confidential (symmetric + asymmetric/JWT) client types.
kind: authentication
layout: security
method: searched
name: Allscripts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allscripts declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Allscripts
provider_slug: allscripts
scheme_count: 0
schemes: []
slug: allscripts-authentication
source_filename: allscripts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs:\n- https://developer.veradigm.com/Fhir/SMARTonFHIR\n- https://developer.veradigm.com/Fhir/ProcessOverview\nsource: >-\n  https://developer.veradigm.com/Fhir/SMARTonFHIR, https://developer.veradigm.com/Fhir/ProcessOverview,\n  plus the live CapabilityStatement (conformance/allscripts-fhir-r4-capabilitystatement.json) and\n  SMART configuration (well-known/allscripts-smart-configuration.json) fetched from a Veradigm\n  Connect sandbox tenant on 2026-08-14.\ndescription: >-\n  Authentication profile for the Veradigm FHIR R4 API. The API supports SMART on FHIR (HL7 SMART\n  App Launch) OAuth 2.0. Veradigm's own docs describe three distinct authentication paths, and the\n  live smart-configuration document confirms three OAuth grant types and both public and\n  confidential (symmetric + asymmetric/JWT) client types.\n\nsecurity_schemes:\n- name: SMART on FHIR (standalone launch)\n  type: oauth2\n  flow: authorizationCode\n  used_by:\
  \ patient-facing and provider-facing apps launched outside an EHR session\n  authorization_url: \"<tenant-specific — see EndpointDirectory>\"\n  token_url: \"<tenant-specific — see EndpointDirectory>\"\n  example_sandbox:\n    authorization_endpoint: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize\n    token_endpoint: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n  notes: >-\n    Application user selects a healthcare organization, then authenticates with EHR credentials\n    (provider apps) or patient-portal credentials such as FollowMyHealth/AHC (patient apps). A\n    provider app may need to prompt for a patient selection when the patient is not embedded in\n    the token response.\n- name: SMART on FHIR (EHR launch)\n  type: oauth2\n  flow: authorizationCode\n  used_by: apps launched from inside the Veradigm EHR UI (Veradigm Connect Integrator tier or above)\n  notes: >-\n    The EHR passes\
  \ `iss` (FHIR endpoint URL) and `launch` (temporary launch authorization code) to\n    the app per the HL7 SMART EHR-launch sequence.\n- name: SMART on FHIR Backend Services (system callers)\n  type: oauth2\n  flow: clientCredentials\n  auth_method: private_key_jwt (JWT client assertion, asymmetric)\n  used_by: server-to-server / System app type — e.g. an insurance company polling appointments for\n    prior authorization, or bulk-data extraction jobs\n  notes: >-\n    Requires backend authentication via a JWKS endpoint; Veradigm processes certificate/key\n    rotation. Client presents a `client_assertion` (JWT signed with a CA-signed private key) plus\n    `client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer`. Only System\n    app types may request bulk data.\n- name: User/provider auth\n  type: http\n  scheme: EHR application credentials (via OAuth 2.0 authorization_code)\n  used_by: human provider users\n- name: Patient portal auth\n  type: http\n  scheme:\
  \ Patient portal credentials — FollowMyHealth or AHC (via OAuth 2.0 authorization_code)\n  used_by: human patient users\n\noauth2_grant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n\nclient_types_supported:\n- client-public\n- client-confidential-symmetric\n- client-confidential-asymmetric\n\napp_registration:\n  portal: https://developer.veradigm.com/\n  process: >-\n    Developer registers a FHIR application in the Veradigm Connect portal (My FHIR Applications),\n    selecting an App Type of Patient, Provider, or System — this determines who can license/see\n    the app and whether it may request bulk data (System only). Client organizations then license\n    the registered app before it can connect to their environment (Endpoint Directory /\n    Client License Management Portal).\n  credentials_issued:\n  - Client ID\n  - Secret\n  - Secret Expiration Date\n\nresponse_types_supported:\n- code\n- token\n- id_token\n- id_token token\n- code id_token\n\
  - code token\n- code id_token token\n\ntoken_format: JWT bearer token, presented in the Authorization header\nidentity_layer: OpenID Connect (sso-openid-connect capability; openid/fhirUser/profile scopes supported)\n\nunity_api_authentication:\n  type: HTTP Basic (username/password)\n  mechanism: Credentials issued by Veradigm during Integrator application registration/certification\n  formats: [REST/JSON, SOAP/XML]\n  source: https://developer.allscripts.com/ (legacy Unity API docs — host now unreachable, see\n    security/allscripts-domain-security.yml)\n  note: >-\n    developer.allscripts.com (the Unity API doc host) timed out on every probe run 2026-08-14; this\n    entry is carried forward from the prior enrichment pass and could not be re-verified this round.\n\ndeprecated:\n- name: DSTU2\n  status: unsupported\n  since: '2025-06-01'\n  note: >-\n    Veradigm no longer provides technical support for DSTU2 FHIR applications as of 2025-06-01.\n    The API endpoint is not turned off,\
  \ but no support or issue resolution is provided. R4 is the\n    current/supported FHIR version.\n\ncross_links:\n  scopes: scopes/allscripts-scopes.yml\n  conformance: conformance/allscripts-conformance.yml\n  lifecycle: lifecycle/allscripts-lifecycle.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts/refs/heads/main/authentication/allscripts-authentication.yml
summary_line: 0 schemes
tags:
- Healthcare IT
- EHR
- FHIR
- Clinical Data
- Practice Management
- HL7
---
