---
api_key_in: []
api_specs:
- filename: emis-health-partner-api-openapi.json
  format: json
  label: EMIS Partner API (PAPI)
  slug: emis-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/openapi/emis-health-partner-api-openapi.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Emis Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- authorizationCodePKCE
- resourceOwnerPassword
overview: EMIS Health secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, authorizationCodePKCE, and resourceOwnerPassword flow(s).
provider_name: EMIS Health
provider_slug: emis-health
scheme_count: 2
schemes:
- applied_to: all 38 partner operations (every operation also accepts OAuth2CodeEMIS-X-GP-PAPI)
  bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/emis-health-partner-api-openapi.json
  type: http
- flows:
  - authorizationUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token
  name: OAuth2CodeEMIS-X-GP-PAPI
  sources:
  - openapi/emis-health-partner-api-openapi.json
  type: oauth2
slug: emis-health-authentication
source_filename: emis-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/emis-health-partner-api-openapi.json\ndocs: https://docs.partner.emis-x.uk/auth/\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, authorizationCodePKCE, resourceOwnerPassword]\n  token_format: JWT bearer\n  token_validity: ~1 hour (issuer may change at any time)\n  identity_provider: Microsoft Entra External ID / Azure AD B2C (identity.stg.emis-x.uk)\n  extra_authorization: >-\n    Access tokens carry an \"authorizations\" JWT claim array of ERN-scoped grants\n    (e.g. clinical-cr.read, clinical-cr.write) plus userERN / orgERN / orgName\n    identity context, governing EMIS-X clinical record access per partner agreement.\nflows_documented:\n- flow: client_credentials\n  client: Machine-to-machine, confidential client\n  user_present: false\n  tokens: access\n- flow: authorization_code\n  client: Web app, confidential client\n  user_present:\
  \ true\n  tokens: [id, access, refresh]\n- flow: authorization_code_pkce\n  client: Mobile / SPA / desktop, public client\n  user_present: true\n  tokens: [id, access, refresh]\n- flow: resource_owner_password\n  client: Automated testing only (not for production)\n  user_present: false\n  tokens: [access, refresh]\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: all 38 partner operations (every operation also accepts OAuth2CodeEMIS-X-GP-PAPI)\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- name: OAuth2CodeEMIS-X-GP-PAPI\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    scopes: 7\n    authorizationUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/authorize\n    tokenUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token\n  sources: [openapi/emis-health-partner-api-openapi.json]\nrequest_context:\n  header: applicationId\n\
  \  required: true\n  note: Every partner operation requires an applicationId header identifying the calling partner application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/authentication/emis-health-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- United Kingdom
- EHR
- EMR
- Interoperability
- HL7
- FHIR
- Primary Care
- NHS
- Clinical Data
- Electronic Patient Record
---
