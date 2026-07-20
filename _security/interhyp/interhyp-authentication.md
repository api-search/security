---
api_key_in:
- header
api_specs:
- filename: interhyp-submission-openapi.yml
  format: yaml
  label: Interhyp Submission API
  slug: interhyp-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-submission-openapi.yml
- filename: interhyp-submission-documents-openapi.yml
  format: yaml
  label: Interhyp Submission Documents API
  slug: interhyp-submission-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-submission-documents-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Interhyp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interhyp secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interhyp
provider_slug: interhyp
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token in JSON Web Token format. Retrieved from the Authorization API using client credentials, then sent in the Authorization header on each request until it expires or is revoked.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/interhyp-submission-openapi.yml
  - openapi/interhyp-submission-documents-openapi.yml
  type: http
- description: Partner API key issued by Interhyp, passed in the Api-Key header on every request to identify and authorize the client application.
  in: header
  name: StandardApiKey
  parameter: Api-Key
  sources:
  - openapi/interhyp-submission-openapi.yml
  type: apiKey
slug: interhyp-authentication
source_filename: interhyp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/interhyp-submission-openapi.yml, openapi/interhyp-submission-documents-openapi.yml\ndocs: https://developer.ehyphome.de/first-steps\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Every request carries two credentials: an Api-Key header identifying the\n    partner application, and an OAuth 2.0 JWT bearer access token in the\n    Authorization header. Both the API key and the OAuth client credentials are\n    generated in the Interhyp Developer Studio. An active partnership agreement\n    with Prohyp is required to obtain credentials.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    OAuth 2.0 access token in JSON Web Token format. Retrieved from the\n    Authorization API using client credentials, then sent in the Authorization\n    header on each request until it expires or is revoked.\n  sources:\n  - openapi/interhyp-submission-openapi.yml\n\
  \  - openapi/interhyp-submission-documents-openapi.yml\n- name: StandardApiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: >-\n    Partner API key issued by Interhyp, passed in the Api-Key header on every\n    request to identify and authorize the client application.\n  sources:\n  - openapi/interhyp-submission-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/authentication/interhyp-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Fintech
- Mortgage
- Lending
- Baufinanzierung
- Real Estate
- Banking
- Germany
- API First
---
