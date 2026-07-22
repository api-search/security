---
api_key_in:
- query
api_specs:
- filename: pixlee-content-api-openapi.yml
  format: yaml
  label: Pixlee Content API
  slug: pixlee-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixlee/refs/heads/main/openapi/pixlee-content-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pixlee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixlee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixlee
provider_slug: pixlee
scheme_count: 1
schemes:
- description: Pixlee ACCOUNT API KEY (read) or ACCOUNT PRIVATE API KEY (write). Found under the API tab in Pixlee account settings.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/pixlee-content-api-openapi.yml
  type: apiKey
slug: pixlee-authentication
source_filename: pixlee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pixlee-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Pixlee ACCOUNT API KEY (read) or ACCOUNT PRIVATE API KEY (write). Found under\n    the API tab in Pixlee account settings.\n  sources:\n  - openapi/pixlee-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixlee/refs/heads/main/authentication/pixlee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- User Generated Content
- Social Commerce
- Visual Marketing
- Content
- Media
- eCommerce
- Widgets
- Emplifi
---
