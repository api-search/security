---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bonterra Fka Everyaction Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bonterra (fka EveryAction) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bonterra (fka EveryAction)
provider_slug: bonterra-fka-everyaction
scheme_count: 1
schemes:
- database_modes:
    '0': My Voters (voter-file data)
    '1': My Campaign (CRM without voter file)
  example_password: 7c9e6679-7425-40de-944b-e07fc1f90ae7|1
  header: Authorization
  in: header
  name: BasicAuth
  password_format: '{apiKey}|{databaseMode}'
  scheme: basic
  sources:
  - docs
  type: http
  username: application-name
slug: bonterra-fka-everyaction-authentication
source_filename: bonterra-fka-everyaction-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.everyaction.com/reference/authentication\ndocs: https://docs.everyaction.com/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  notes: >-\n    HTTP Basic authentication. Username is the developer-assigned Application Name; password is the\n    API key with a database-mode suffix appended after a pipe. Standard Base64 Authorization: Basic\n    header. There is no OAuth or scope surface on the EveryAction/NGP VAN API.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  username: application-name\n  password_format: \"{apiKey}|{databaseMode}\"\n  database_modes:\n    '0': My Voters (voter-file data)\n    '1': My Campaign (CRM without voter file)\n  example_password: \"7c9e6679-7425-40de-944b-e07fc1f90ae7|1\"\n  sources:\n  - docs\nnotes:\n- API keys are tied to a specific developer and application and must not be shared, exposed in\n\
  \  client-side code, or committed to public repositories.\n- The GET /apiKeyProfiles introspection endpoint returns information about the API key in use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonterra-fka-everyaction/refs/heads/main/authentication/bonterra-fka-everyaction-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- API
- CRM
- Nonprofit
- Fundraising
- Advocacy
- Political
- Voter Engagement
- Donor Management
- Organizing
---
