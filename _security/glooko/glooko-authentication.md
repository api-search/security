---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Glooko Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Glooko secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Glooko
provider_slug: glooko
scheme_count: 1
schemes:
- description: 'Glooko''s EHR integration program uses SMART on FHIR, which layers OAuth 2.0 authorization-code flow over HL7 FHIR for EHR-launched and standalone healthcare applications. Access is partner-gated: integration credentials are provisioned through the Glooko API and EHR Integration Portal (developers.glooko.com) rather than self-serve signup.'
  flow: authorizationCode
  name: SMARTonFHIR
  scheme: SMART on FHIR (OAuth 2.0)
  sources:
  - https://glooko.com/partners/
  type: oauth2
slug: glooko-authentication
source_filename: glooko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.glooko.com/\ndocs:\n- https://developers.glooko.com/\n- https://glooko.com/partners/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  standards:\n  - SMART on FHIR\n  - OAuth 2.0\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  scheme: SMART on FHIR (OAuth 2.0)\n  flow: authorizationCode\n  description: >-\n    Glooko's EHR integration program uses SMART on FHIR, which layers OAuth 2.0\n    authorization-code flow over HL7 FHIR for EHR-launched and standalone\n    healthcare applications. Access is partner-gated: integration credentials are\n    provisioned through the Glooko API and EHR Integration Portal\n    (developers.glooko.com) rather than self-serve signup.\n  sources:\n  - https://glooko.com/partners/\nnotes: >-\n  No public OpenAPI/Swagger specification is published (developers.glooko.com is a\n  partner-gated single-page app), so this profile is derived from Glooko's\n\
  \  documented SMART on FHIR / OAuth 2.0 integration model rather than a\n  machine-readable securityScheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glooko/refs/heads/main/authentication/glooko-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Diabetes
- Diabetes Management
- Healthcare
- Digital Health
- Remote Patient Monitoring
- Medical Devices
- EHR Integration
- FHIR
- Interoperability
- Chronic Care
- Life Sciences
---
