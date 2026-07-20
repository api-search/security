---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Handshake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Handshake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Handshake
provider_slug: handshake
scheme_count: 1
schemes:
- description: Every EDU API request must send an x-api-key header carrying the institution's API key. Keys are issued and managed from the Handshake Developer Portal (edu-api.joinhandshake.com) in the Subscriptions section. A regenerated key must be enabled by the Handshake Technical Support team before it will authenticate.
  in: header
  name: x-api-key
  parameter_name: x-api-key
  sources:
  - docs
  type: apiKey
slug: handshake-authentication
source_filename: handshake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.joinhandshake.com/hc/en-us/articles/31061076506391-Getting-Started-with-EDU-API\ndocs: https://support.joinhandshake.com/hc/en-us/sections/31055822163351-API\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Every EDU API request must send an x-api-key header carrying the institution's API\n    key. Keys are issued and managed from the Handshake Developer Portal\n    (edu-api.joinhandshake.com) in the Subscriptions section. A regenerated key must be\n    enabled by the Handshake Technical Support team before it will authenticate.\n  sources:\n  - docs\nnotes: >-\n  EDU API access is institution-scoped and read-only, currently in beta, and gated to\n  Career Services partners (request access via your Handshake Relationship Manager). No\n  public OpenAPI is published, so\
  \ this profile is captured from the developer\n  documentation rather than derived from a spec. The developer portal also references an\n  OAuth playground and GraphQL/API explorer surfaces available to authenticated partners.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handshake/refs/heads/main/authentication/handshake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Hr Tech
- Careers
- Recruiting
- Higher Education
- Talent
- Students
- Jobs
---
