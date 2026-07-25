---
api_key_in: []
api_specs:
- filename: shuffle-administration-api-openapi.yml
  format: yaml
  label: Shuffle Administration API
  slug: shuffle-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-administration-api-openapi.yml
- filename: shuffle-apps-api-openapi.yml
  format: yaml
  label: Shuffle Apps API
  slug: shuffle-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-apps-api-openapi.yml
- filename: shuffle-datastore-api-openapi.yml
  format: yaml
  label: Shuffle Datastore API
  slug: shuffle-datastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-datastore-api-openapi.yml
- filename: shuffle-files-api-openapi.yml
  format: yaml
  label: Shuffle Files API
  slug: shuffle-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-files-api-openapi.yml
- filename: shuffle-notifications-api-openapi.yml
  format: yaml
  label: Shuffle Notifications API
  slug: shuffle-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-notifications-api-openapi.yml
- filename: shuffle-organizations-api-openapi.yml
  format: yaml
  label: Shuffle Organizations API
  slug: shuffle-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-organizations-api-openapi.yml
- filename: shuffle-triggers-api-openapi.yml
  format: yaml
  label: Shuffle Triggers API
  slug: shuffle-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-triggers-api-openapi.yml
- filename: shuffle-users-api-openapi.yml
  format: yaml
  label: Shuffle Users API
  slug: shuffle-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-users-api-openapi.yml
- filename: shuffle-workflows-api-openapi.yml
  format: yaml
  label: Shuffle Workflows API
  slug: shuffle-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shuffle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shuffle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shuffle
provider_slug: shuffle
scheme_count: 1
schemes:
- description: 'API key obtained from Shuffle profile settings. Include as: Authorization: Bearer <APIKEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/shuffle-openapi.yml
  type: http
slug: shuffle-authentication
source_filename: shuffle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shuffle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key obtained from Shuffle profile settings. Include as: Authorization: Bearer\n    <APIKEY>'\n  sources:\n  - openapi/shuffle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/authentication/shuffle-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Workflows
- Automation
- SOAR
- Orchestration
- Open Source
---
