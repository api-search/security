---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pantheon-run-ai-api-openapi.yml
  format: yaml
  label: Pantheon AI API
  slug: pantheon-run-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-ai-api-openapi.yml
- filename: pantheon-run-chats-api-openapi.yml
  format: yaml
  label: Pantheon Chats API
  slug: pantheon-run-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-chats-api-openapi.yml
- filename: pantheon-run-contacts-api-openapi.yml
  format: yaml
  label: Pantheon Contacts API
  slug: pantheon-run-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-contacts-api-openapi.yml
- filename: pantheon-run-deals-api-openapi.yml
  format: yaml
  label: Pantheon Deals API
  slug: pantheon-run-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-deals-api-openapi.yml
- filename: pantheon-run-files-api-openapi.yml
  format: yaml
  label: Pantheon Files API
  slug: pantheon-run-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-files-api-openapi.yml
- filename: pantheon-run-r-api-openapi.yml
  format: yaml
  label: Pantheon R API
  slug: pantheon-run-r-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-r-api-openapi.yml
- filename: pantheon-run-records-api-openapi.yml
  format: yaml
  label: Pantheon Records API
  slug: pantheon-run-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-records-api-openapi.yml
- filename: pantheon-run-usage-api-openapi.yml
  format: yaml
  label: Pantheon Usage API
  slug: pantheon-run-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pantheon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pantheon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pantheon
provider_slug: pantheon-run
scheme_count: 1
schemes:
- description: 'Developer API key — Authorization: Bearer pk_live_...'
  name: apiKeyAuth
  scheme: bearer
  sources:
  - openapi/pantheon-run-openapi.json
  type: http
slug: pantheon-run-authentication
source_filename: pantheon-run-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pantheon-run-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Developer API key — Authorization: Bearer pk_live_...'\n  sources:\n  - openapi/pantheon-run-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/pantheon-run/authentication/pantheon-run-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Messaging
- Unified Inbox
- Customer Engagement
- Communications
---
