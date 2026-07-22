---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Turnitin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turnitin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Turnitin
provider_slug: turnitin
scheme_count: 1
schemes:
- description: TCA authenticates each request with an API key. An API key exists under an "integration instance"; a tenant can have multiple integration instances (typically at least one Sandbox and one Production instance). All data created within an integration instance is scoped to that instance. The key is issued from the Turnitin administrator console for the integration instance.
  docs: https://developers.turnitin.com/turnitin-core-api
  in: header
  name: tca-api-key
  type: apiKey
slug: turnitin-authentication
source_filename: turnitin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://developers.turnitin.com/turnitin-core-api and\n  https://developers.turnitin.com/turnitin-core-api/faq — the Turnitin Core API\n  (TCA) developer guides. No public OpenAPI is available (the API Reference is\n  behind a customer login), so this profile is captured from the published\n  developer documentation rather than derived from a spec.\napi: Turnitin Core API (TCA)\nsummary:\n  types:\n    - apiKey\nschemes:\n  - name: tca-api-key\n    type: apiKey\n    in: header\n    description: >-\n      TCA authenticates each request with an API key. An API key exists under an\n      \"integration instance\"; a tenant can have multiple integration instances\n      (typically at least one Sandbox and one Production instance). All data\n      created within an integration instance is scoped to that instance. The key\n      is issued from the Turnitin administrator console for the integration\n      instance.\n    docs:\
  \ https://developers.turnitin.com/turnitin-core-api\nrequired_headers:\n  - name: X-Turnitin-Integration-Name\n    description: >-\n      Identifies the integrating platform. Set to the name of your LMS or\n      software. Required on TCA requests.\n  - name: X-Turnitin-Integration-Version\n    description: >-\n      The version of your integrating platform/software. Required on TCA\n      requests; also used by Turnitin to track integration versions.\nnotes: >-\n  TCA is a RESTful API. Turnitin also supports LTI (Learning Tools\n  Interoperability) as a separate integration path\n  (https://developers.turnitin.com/learning-tools-interoperability), which uses\n  the LTI/OAuth handshake rather than the TCA API key. This profile covers the\n  TCA REST surface only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turnitin/refs/heads/main/authentication/turnitin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Education
- EdTech
- Academic Integrity
- Plagiarism Detection
- Similarity
- AI Detection
- Assessment
- Research Integrity
- Publishing
- LTI
---
