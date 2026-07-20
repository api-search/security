---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Carbon Black Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carbon Black secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carbon Black
provider_slug: carbon-black
scheme_count: 1
schemes:
- description: API Id/Secret credential pair passed directly in the X-Auth-Token request header. Requests also require Content-Type application/json.
  header_name: X-Auth-Token
  in: header
  name: XAuthToken
  source: docs
  type: apiKey
  value_format: '{API Secret}/{API Id}'
slug: carbon-black-authentication
source_filename: carbon-black-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.carbonblack.com/reference/carbon-black-cloud/authentication/\ndocs: https://developer.carbonblack.com/reference/carbon-black-cloud/authentication/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: Carbon Black Cloud does not use OAuth. Access is granted via an API Key\n    (API Id + API Secret) created under Settings > API Access with a Custom Access\n    Level scoped to least privilege.\nschemes:\n- name: XAuthToken\n  type: apiKey\n  in: header\n  header_name: X-Auth-Token\n  value_format: '{API Secret}/{API Id}'\n  description: API Id/Secret credential pair passed directly in the X-Auth-Token\n    request header. Requests also require Content-Type application/json.\n  source: docs\nhosts:\n- environment: Prod 01\n  url: https://dashboard.confer.net\n- environment: Prod 02\n  url: https://defense.conferdeploy.net\n- environment: Prod 05\n  url: https://defense-prod05.conferdeploy.net\n\
  - environment: Prod 06 (EU)\n  url: https://defense-eu.conferdeploy.net\n- environment: Prod NRT (Asia-Pacific / Tokyo)\n  url: https://defense-prodnrt.conferdeploy.net\n- environment: Prod SYD (Sydney)\n  url: https://defense-prodsyd.conferdeploy.net\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-black/refs/heads/main/authentication/carbon-black-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Endpoint Security
- EDR
- Threat Detection
- Cybersecurity
- Cloud Security
---
