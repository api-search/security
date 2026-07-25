---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 1Uphealth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: 1upHealth secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: 1upHealth
provider_slug: 1uphealth
scheme_count: 2
schemes:
- description: SMART-on-FHIR OAuth 2.0 as advertised in each CapabilityStatement's security.extension oauth-uris block.
  flows:
  - authorizationUrl: https://auth.1up.health/oauth2/authorize/system
    description: SMART app-launch / patient-authorization flow for user-facing apps.
    flow: authorizationCode
    tokenUrl: https://auth.1up.health/oauth2/token
  - description: System (backend) authorization for server-to-server access and Bulk Data ($export) jobs.
    flow: clientCredentials
    tokenUrl: https://auth.1up.health/oauth2/token
  name: SMARTonFHIR
  sources:
  - fhir/1uphealth-fhir-r4-capabilitystatement.json
  - fhir/1uphealth-fhir-stu3-capabilitystatement.json
  - fhir/1uphealth-fhir-dstu2-conformance.json
  type: oauth2
- description: Product-specific OpenID Connect / Keycloak realms fronting the CMS solution APIs (Provider Access, Payer-to-Payer, Electronic Prior Authorization). Credentials are issued from the 1up Dev Portal (Create a Client).
  flows:
  - description: Provider Access & Payer-to-Payer (dev-portal realm).
    flow: clientCredentials
    tokenUrl: https://gateway.1up.health/auth/realms/dev-portal/protocol/openid-connect/token
  - description: Electronic Prior Authorization production realm.
    flow: clientCredentials
    tokenUrl: https://gateway.1upcoreprod.com/auth/realms/epa-prod/protocol/openid-connect/token
  - description: Electronic Prior Authorization UAT/demo realm.
    flow: clientCredentials
    tokenUrl: https://gateway.1upcoreuat.com/auth/realms/epa-uat/protocol/openid-connect/token
  name: KeycloakClientCredentials
  sources:
  - https://docs.1up.health/docs/get-started/o-auth
  type: oauth2
slug: 1uphealth-authentication
source_filename: 1uphealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  fhir/1uphealth-fhir-r4-capabilitystatement.json (SMART-on-FHIR oauth-uris) +\n  https://docs.1up.health/docs/get-started/o-auth\ndocs: https://docs.1up.health/docs/get-started/o-auth\nsummary:\n  types: [oauth2]\n  model: SMART-on-FHIR\n  oauth2_flows: [authorizationCode, clientCredentials]\n  api_key_in: []\n  notes: >-\n    All 1up FHIR endpoints are secured with SMART-on-FHIR OAuth 2.0 (declared in the\n    live CapabilityStatement restful-security-service = SMART-on-FHIR). System-to-system\n    and bulk-data integrations use the OAuth 2.0 client_credentials grant; patient- and\n    user-facing apps use the SMART authorization_code (app launch) flow. CMS solution\n    products (Provider Access, Payer-to-Payer, Electronic Prior Authorization) are\n    fronted by Keycloak realms on the 1up gateway with per-environment token endpoints.\nschemes:\n  - name: SMARTonFHIR\n    type: oauth2\n    description: >-\n      SMART-on-FHIR\
  \ OAuth 2.0 as advertised in each CapabilityStatement's\n      security.extension oauth-uris block.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.1up.health/oauth2/authorize/system\n        tokenUrl: https://auth.1up.health/oauth2/token\n        description: SMART app-launch / patient-authorization flow for user-facing apps.\n      - flow: clientCredentials\n        tokenUrl: https://auth.1up.health/oauth2/token\n        description: >-\n          System (backend) authorization for server-to-server access and Bulk Data\n          ($export) jobs.\n    sources:\n      - fhir/1uphealth-fhir-r4-capabilitystatement.json\n      - fhir/1uphealth-fhir-stu3-capabilitystatement.json\n      - fhir/1uphealth-fhir-dstu2-conformance.json\n  - name: KeycloakClientCredentials\n    type: oauth2\n    description: >-\n      Product-specific OpenID Connect / Keycloak realms fronting the CMS solution APIs\n      (Provider Access, Payer-to-Payer, Electronic Prior Authorization).\
  \ Credentials are\n      issued from the 1up Dev Portal (Create a Client).\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://gateway.1up.health/auth/realms/dev-portal/protocol/openid-connect/token\n        description: Provider Access & Payer-to-Payer (dev-portal realm).\n      - flow: clientCredentials\n        tokenUrl: https://gateway.1upcoreprod.com/auth/realms/epa-prod/protocol/openid-connect/token\n        description: Electronic Prior Authorization production realm.\n      - flow: clientCredentials\n        tokenUrl: https://gateway.1upcoreuat.com/auth/realms/epa-uat/protocol/openid-connect/token\n        description: Electronic Prior Authorization UAT/demo realm.\n    sources:\n      - https://docs.1up.health/docs/get-started/o-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1uphealth/refs/heads/main/authentication/1uphealth-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Payer
- Claims
- Patient Access
- Health Data
---
