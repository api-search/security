---
api_key_in: []
api_specs:
- filename: elbo-ai-inc-puppetry-openapi-original.json
  format: json
  label: Puppetry Developer API
  slug: puppetry-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elbo-ai-inc/refs/heads/main/openapi/elbo-ai-inc-puppetry-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elbo Ai Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: ELBO AI, INC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ELBO AI, INC
provider_slug: elbo-ai-inc
scheme_count: 1
schemes:
- bearerFormat: Puppetry API key
  description: 'Use the Authorization header with a live Puppetry API key: Bearer [example key]'
  name: developerApiKey
  scheme: bearer
  sources:
  - openapi/elbo-ai-inc-puppetry-openapi-original.json
  type: http
slug: elbo-ai-inc-authentication
source_filename: elbo-ai-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/elbo-ai-inc-puppetry-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: developerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Puppetry API key\n  description: 'Use the Authorization header with a live Puppetry API key: Bearer [example key]'\n  sources:\n  - openapi/elbo-ai-inc-puppetry-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elbo-ai-inc/refs/heads/main/authentication/elbo-ai-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video
- Text to Speech
- Voice
- Generative AI
- Avatars
- Content Creation
- Developer API
- MCP
---
