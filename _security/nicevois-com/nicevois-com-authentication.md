---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nicevois-com-account-api-openapi.yml
  format: yaml
  label: NiceVois Account API
  slug: nicevois-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nicevois-com/openapi/nicevois-com-account-api-openapi.yml
- filename: nicevois-com-conversion-api-openapi.yml
  format: yaml
  label: NiceVois Conversion API
  slug: nicevois-com-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nicevois-com/openapi/nicevois-com-conversion-api-openapi.yml
- filename: nicevois-com-discovery-api-openapi.yml
  format: yaml
  label: NiceVois Discovery API
  slug: nicevois-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nicevois-com/openapi/nicevois-com-discovery-api-openapi.yml
- filename: nicevois-com-free-audio-tools-api-openapi.yml
  format: yaml
  label: NiceVois Free audio tools API
  slug: nicevois-com-free-audio-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nicevois-com/openapi/nicevois-com-free-audio-tools-api-openapi.yml
- filename: nicevois-com-training-api-openapi.yml
  format: yaml
  label: NiceVois Training API
  slug: nicevois-com-training-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nicevois-com/openapi/nicevois-com-training-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NiceVois Authentication
name_suffix: Authentication
oauth_flows: []
overview: NiceVois secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NiceVois
provider_slug: nicevois-com
scheme_count: 1
schemes:
- bearerFormat: NiceVois agent key (nvk_...) or OAuth 2.1 access token
  description: An agent key the customer creates at https://nicevois.com/account, or an OAuth-connected NiceVois access token. A key acts as that account, with its plan, passes and limits. Never place either credential in prompts, logs, URLs, or tool output.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nicevois-com-openapi.json
  type: http
slug: nicevois-com-authentication
source_filename: nicevois-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nicevois-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: NiceVois agent key (nvk_...) or OAuth 2.1 access token\n  description: An agent key the customer creates at https://nicevois.com/account, or an OAuth-connected\n    NiceVois access token. A key acts as that account, with its plan, passes and limits. Never\n    place either credential in prompts, logs, URLs, or tool output.\n  sources:\n  - openapi/nicevois-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nicevois-com/authentication/nicevois-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Voice
- Audio
- Machine Learning
- Software-as-a-Service
---
