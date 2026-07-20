---
api_key_in:
- header
auth_types:
- apiKey
description: 'Crunchtime Inventory & Labor / Cruise APIs use custom header-based token authentication. Every request carries four headers: an access token plus the site name and an Application User''s id and password. Tokens are minted per Application User in Enterprise Manager (Security > Application Users > API Tokens) and separate test and production tokens are issued. There is no OAuth2 or OpenID Connect surface, so this repo has no scopes/ artifact.'
kind: authentication
layout: security
method: searched
name: Crunchtime Information Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crunchtime Information Systems secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crunchtime Information Systems
provider_slug: crunchtime-information-systems
scheme_count: 4
schemes:
- description: Secure access token for API authentication. Issued per Application User in Enterprise Manager; distinct test and production tokens exist.
  in: header
  name: authenticationtoken
  parameter_name: authenticationtoken
  sources:
  - https://developer.crunchtime.com/reference/getalllocationsv1usingget
  type: apiKey
- description: Crunchtime site identifier (the portion of the customer URL before .net-chef.com), designating the test or production environment.
  in: header
  name: sitename
  parameter_name: sitename
  sources:
  - https://developer.crunchtime.com/reference/getalllocationsv1usingget
  type: apiKey
- description: Application User ID used for the request.
  in: header
  name: userid
  parameter_name: userid
  sources:
  - https://developer.crunchtime.com/reference/getalllocationsv1usingget
  type: apiKey
- description: Application User password paired with the userid header.
  in: header
  name: password
  parameter_name: password
  sources:
  - https://developer.crunchtime.com/reference/getalllocationsv1usingget
  type: apiKey
slug: crunchtime-information-systems-authentication
source_filename: crunchtime-information-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.crunchtime.com/docs/getting-started-with-apis\ndocs: https://developer.crunchtime.com/docs/getting-started-with-apis\ndescription: >-\n  Crunchtime Inventory & Labor / Cruise APIs use custom header-based token\n  authentication. Every request carries four headers: an access token plus the\n  site name and an Application User's id and password. Tokens are minted per\n  Application User in Enterprise Manager (Security > Application Users > API\n  Tokens) and separate test and production tokens are issued. There is no OAuth2\n  or OpenID Connect surface, so this repo has no scopes/ artifact.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: authenticationtoken\n  type: apiKey\n  in: header\n  parameter_name: authenticationtoken\n  description: >-\n    Secure access token for API authentication. Issued per Application User in\n    Enterprise Manager; distinct test and\
  \ production tokens exist.\n  sources: [https://developer.crunchtime.com/reference/getalllocationsv1usingget]\n- name: sitename\n  type: apiKey\n  in: header\n  parameter_name: sitename\n  description: >-\n    Crunchtime site identifier (the portion of the customer URL before\n    .net-chef.com), designating the test or production environment.\n  sources: [https://developer.crunchtime.com/reference/getalllocationsv1usingget]\n- name: userid\n  type: apiKey\n  in: header\n  parameter_name: userid\n  description: Application User ID used for the request.\n  sources: [https://developer.crunchtime.com/reference/getalllocationsv1usingget]\n- name: password\n  type: apiKey\n  in: header\n  parameter_name: password\n  description: Application User password paired with the userid header.\n  sources: [https://developer.crunchtime.com/reference/getalllocationsv1usingget]\ncredential_management:\n  console: Enterprise Manager > Security > Application Users > API Tokens\n  self_service: >-\n    A\
  \ self-service API token management process (added 2026-04-28) lets users\n    create and manage tokens directly in Enterprise Manager without Support tickets.\n  guidance: >-\n    Crunchtime recommends creating a dedicated Application User (e.g. \"API User\")\n    rather than authenticating as a named human user.\n  contact: apiquestions@crunchtime.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchtime-information-systems/refs/heads/main/authentication/crunchtime-information-systems-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Restaurant
- Food Service
- Hospitality
- Inventory Management
- Labor Scheduling
- Operations Management
- Back Office
- Supply Chain
- API
---
