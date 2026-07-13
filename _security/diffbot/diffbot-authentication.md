---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Diffbot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diffbot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diffbot
provider_slug: diffbot
scheme_count: 1
schemes:
- in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/diffbot-openapi.yml
  type: apiKey
slug: diffbot-authentication
source_filename: diffbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/diffbot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/diffbot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/authentication/diffbot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Extraction
- Harvesting
- Scraping
- Web
---
