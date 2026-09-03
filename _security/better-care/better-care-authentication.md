---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Better Care Authentication
name_suffix: Authentication
oauth_flows: []
overview: Better secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Better
provider_slug: better-care
scheme_count: 1
schemes:
- applies_to: Better Platform openEHR REST API
  confidence: medium
  evidence: Better's own Apache-2.0 openEHR REST integration-test suite configures the server under test with `auth.basic.username` and `auth.basic.password`, documented as "Username for basic auth. If not set, there is no authentication". That is the authentication mode Better itself exercises against a deployed openEHR REST endpoint.
  name: basic
  scheme: basic
  sources:
  - https://github.com/better-care/openehr-rest-tests
  type: http
slug: better-care-authentication
source_filename: better-care-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://github.com/better-care/openehr-rest-tests ;\n  https://docs.better.care/studio/build-in-studio/connecting-data ;\n  https://github.com/better-care/better-abac-server ;\n  https://docs.better.care/studio/release-notes/release-3-15\ndocs: null\ndocs_note: >-\n  Better publishes NO public authentication reference for its own API. The Better Platform\n  documentation tree (https://docs.better.care/platform/) 302s into\n  login.microsoftonline.com SAML, and derive-authentication.py found no securitySchemes because\n  no OpenAPI exists in this repo. Everything below is read from Better's own public source code\n  and public Studio documentation, and is described at that confidence level rather than as a\n  documented contract.\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  confidence: medium\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  applies_to: Better Platform openEHR REST API\n\
  \  sources: ['https://github.com/better-care/openehr-rest-tests']\n  evidence: >-\n    Better's own Apache-2.0 openEHR REST integration-test suite configures the server under test\n    with `auth.basic.username` and `auth.basic.password`, documented as \"Username for basic auth.\n    If not set, there is no authentication\". That is the authentication mode Better itself\n    exercises against a deployed openEHR REST endpoint.\n  confidence: medium\nclient_side_connector_auth:\n  note: >-\n    Distinct from Better's OWN API auth. Better Studio Data Connectors (the outbound HTTP client\n    a form uses to call third-party APIs, introduced in Studio 3.13 as the successor to API\n    Connectors) offer four authentication choices, one of which reuses platform credentials.\n  source: https://docs.better.care/studio/build-in-studio/connecting-data\n  options: [None, Basic, Bearer, EHR Platform credentials]\n  methods: [GET, POST, PUT, PATCH, DELETE]\n  body_types: [json, form-data, x-www-form-urlencoded,\
  \ file/binary]\nauthorization:\n  abac:\n    project: Better ABAC Server\n    url: https://github.com/better-care/better-abac-server\n    license: Apache-2.0\n    last_updated: '2024-09-12'\n    note: >-\n      Better publishes an attribute-based access control server as open source; it is the\n      authorization component of a Better deployment. No public policy reference or scope list\n      is published.\naccount_security:\n  two_factor_authentication:\n    product: Better Studio\n    since: 3.15.0\n    since_date: '2026-04-21'\n    source: https://docs.better.care/studio/release-notes/release-3-15\n  sso:\n    note: >-\n      Better's own documentation, support and status estates sit behind identity providers -\n      docs.better.care/platform redirects to Microsoft Entra (tenant\n      910f2764-a2db-4c62-88c4-a5e70c3365c4) SAML, and better.statuspage.io redirects to Better's\n      Okta. This is evidence of Better's internal IdP, not of customer-facing API auth.\nnot_found:\n- api-key\
  \ issuance documentation\n- OAuth 2.0 / OpenID Connect discovery documents (probed on every host; see well-known/)\n- scope or permission reference (no scopes/ artifact is written - Better has no documented OAuth surface)\n- mutual TLS documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-care/refs/heads/main/authentication/better-care-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- openEHR
- Electronic Health Records
- Clinical Data
- Interoperability
- HL7 FHIR
- Medication Management
- Digital Health
- Low Code
- AQL
- Slovenia
---
