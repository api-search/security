---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cronjob-de-benachrichtigungen-api-openapi.yml
  format: yaml
  label: Cronjob.de Benachrichtigungen API
  slug: cronjob-de-benachrichtigungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-benachrichtigungen-api-openapi.yml
- filename: cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
  format: yaml
  label: Cronjob.de Cronjobs und Heartbeats API
  slug: cronjob-de-cronjobs-und-heartbeats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
- filename: cronjob-de-server-berwachung-und-ssl-api-openapi.yml
  format: yaml
  label: Cronjob.de Serverüberwachung und SSL API
  slug: cronjob-de-server-berwachung-und-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-server-berwachung-und-ssl-api-openapi.yml
- filename: cronjob-de-statusseiten-api-openapi.yml
  format: yaml
  label: Cronjob.de Statusseiten API
  slug: cronjob-de-statusseiten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-statusseiten-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cronjob De Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cronjob.de secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cronjob.de
provider_slug: cronjob-de
scheme_count: 1
schemes:
- description: API key "<user_id>:<token>" from https://www.cronjob.de/loggedin/ki-zugang#ohne-browser
  name: bearer
  scheme: bearer
  sources:
  - openapi/cronjob-de-openapi.json
  type: http
slug: cronjob-de-authentication
source_filename: cronjob-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cronjob-de-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key \"<user_id>:<token>\" from https://www.cronjob.de/loggedin/ki-zugang#ohne-browser\n  sources:\n  - openapi/cronjob-de-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cronjob-de/authentication/cronjob-de-authentication.yml
summary_line: http · 1 scheme
tags:
- Cronjob
- Scheduling
- Automation
- EU-hosted
---
