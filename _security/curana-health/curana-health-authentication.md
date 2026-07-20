---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Curana Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curana Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Curana Health
provider_slug: curana-health
scheme_count: 1
schemes:
- description: OAuth 2.0 member authorization; access tokens scoped per FHIR resource.
  name: OAuth2
  sources:
  - https://curanahealth.com/wp-content/uploads/2026/04/3rd_PARTY_CMS_APIS_v2.2.pdf
  type: oauth2
slug: curana-health-authentication
source_filename: curana-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://curanahealth.com/wp-content/uploads/2026/04/3rd_PARTY_CMS_APIS_v2.2.pdf\ndocs: https://curanahealth.com/interoperability-api/\nsummary:\n  types: [oauth2]\n  standard: SMART on FHIR / OAuth 2.0\n  patient_authorization: true\n  registration_required: true\nnotes: >-\n  The Curana Health Interoperability (Patient Access) API uses OAuth 2.0 for member\n  authorization, consistent with the CMS-9115-F Patient Access API and ONC 21st Century\n  Cures Act requirements. Third-party application owners must register (Sandbox and/or\n  Production) via the Patient API Access form before receiving credentials. Access tokens\n  carry explicitly-declared scopes that gate which FHIR resources an app may read;\n  wildcards are not supported. A member may revoke consent at any time, after which the\n  app's token is invalidated (invalid-token responses). The public Provider Directory\n  surface is reachable without patient authorization\
  \ per CMS rules.\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: OAuth 2.0 member authorization; access tokens scoped per FHIR resource.\n  sources: [https://curanahealth.com/wp-content/uploads/2026/04/3rd_PARTY_CMS_APIS_v2.2.pdf]\nregistration:\n  url: https://curanahealth.com/patient-api-access-form/\n  access_tiers: [Sandbox, Production, Sandbox and Production]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curana-health/refs/heads/main/authentication/curana-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Digital Health
- Healthcare
- FHIR
- Interoperability
- Medicare Advantage
- Senior Living
- Patient Access
- Value-Based Care
- CMS-9115-F
---
