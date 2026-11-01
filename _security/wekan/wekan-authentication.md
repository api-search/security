---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: wekan-attachments-api-openapi.yml
  format: yaml
  label: WeKan Attachments API
  slug: wekan-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-attachments-api-openapi.yml
- filename: wekan-attachmentstoragesettings-api-openapi.yml
  format: yaml
  label: WeKan Attachment Storage Settings API
  slug: wekan-attachmentstoragesettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-attachmentstoragesettings-api-openapi.yml
- filename: wekan-boards-api-openapi.yml
  format: yaml
  label: WeKan Boards API
  slug: wekan-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-boards-api-openapi.yml
- filename: wekan-cardcomments-api-openapi.yml
  format: yaml
  label: WeKan Card Comments API
  slug: wekan-cardcomments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-cardcomments-api-openapi.yml
- filename: wekan-cards-api-openapi.yml
  format: yaml
  label: WeKan Cards API
  slug: wekan-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-cards-api-openapi.yml
- filename: wekan-checklists-api-openapi.yml
  format: yaml
  label: WeKan Checklists API
  slug: wekan-checklists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-checklists-api-openapi.yml
- filename: wekan-dependencies-api-openapi.yml
  format: yaml
  label: WeKan Dependencies API
  slug: wekan-dependencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-dependencies-api-openapi.yml
- filename: wekan-integrations-api-openapi.yml
  format: yaml
  label: WeKan Integrations API
  slug: wekan-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-integrations-api-openapi.yml
- filename: wekan-lists-api-openapi.yml
  format: yaml
  label: WeKan Lists API
  slug: wekan-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-lists-api-openapi.yml
- filename: wekan-login-api-openapi.yml
  format: yaml
  label: WeKan Login API
  slug: wekan-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-login-api-openapi.yml
- filename: wekan-org-api-openapi.yml
  format: yaml
  label: WeKan Org API
  slug: wekan-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-org-api-openapi.yml
- filename: wekan-organizations-api-openapi.yml
  format: yaml
  label: WeKan Organizations API
  slug: wekan-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-organizations-api-openapi.yml
- filename: wekan-problems-api-openapi.yml
  format: yaml
  label: WeKan Problems API
  slug: wekan-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-problems-api-openapi.yml
- filename: wekan-rules-api-openapi.yml
  format: yaml
  label: WeKan Rules API
  slug: wekan-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-rules-api-openapi.yml
- filename: wekan-settings-api-openapi.yml
  format: yaml
  label: WeKan Settings API
  slug: wekan-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-settings-api-openapi.yml
- filename: wekan-swimlanes-api-openapi.yml
  format: yaml
  label: WeKan Swimlanes API
  slug: wekan-swimlanes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-swimlanes-api-openapi.yml
- filename: wekan-team-api-openapi.yml
  format: yaml
  label: WeKan Team API
  slug: wekan-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-team-api-openapi.yml
- filename: wekan-teams-api-openapi.yml
  format: yaml
  label: WeKan Teams API
  slug: wekan-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-teams-api-openapi.yml
- filename: wekan-users-api-openapi.yml
  format: yaml
  label: WeKan Users API
  slug: wekan-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-users-api-openapi.yml
- filename: wekan-checklist-items-api-openapi.yml
  format: yaml
  label: WeKan Checklist Items API
  slug: wekan-checklist-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-checklist-items-api-openapi.yml
- filename: wekan-custom-fields-api-openapi.yml
  format: yaml
  label: WeKan Custom Fields API
  slug: wekan-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-custom-fields-api-openapi.yml
- filename: wekan-event-log-api-openapi.yml
  format: yaml
  label: WeKan Event Log API
  slug: wekan-event-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-event-log-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Wekan Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeKan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WeKan
provider_slug: wekan
scheme_count: 1
schemes:
- in: header
  name: UserSecurity
  parameter: Authorization
  sources:
  - openapi/wekan-meteor3-openapi.yml
  - openapi/wekan-openapi.yml
  type: apiKey
slug: wekan-authentication
source_filename: wekan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/wekan-meteor3-openapi.yml, openapi/wekan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: UserSecurity\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/wekan-meteor3-openapi.yml\n  - openapi/wekan-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/wekan/authentication/wekan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
---
