---
api_key_in: []
api_specs:
- filename: rapidata-openapi-original.json
  format: json
  label: Rapidata API
  slug: rapidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/openapi/rapidata-openapi-original.json
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Rapidata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rapidata secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rapidata
provider_slug: rapidata
scheme_count: 1
schemes:
- description: OpenID Connect connection flow
  name: OpenIdConnect
  openIdConnectUrl: https://auth.rapidata.ai/.well-known/openid-configuration
  sources:
  - openapi/rapidata-openapi-original.json
  type: openIdConnect
slug: rapidata-authentication
source_filename: rapidata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/rapidata-openapi-original.json\nsummary:\n  types:\n  - openIdConnect\nschemes:\n- name: OpenIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.rapidata.ai/.well-known/openid-configuration\n  description: OpenID Connect connection flow\n  sources:\n  - openapi/rapidata-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/authentication/rapidata-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Human Feedback
- Data Labeling
- Annotation
- RLHF
- Model Evaluation
- Machine Learning
- AI
- Crowdsourcing
- Preference Data
---
