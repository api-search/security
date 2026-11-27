---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bombbomb-accounts-api-openapi.yml
  format: yaml
  label: BombBomb Accounts API
  slug: bombbomb-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-accounts-api-openapi.yml
- filename: bombbomb-automations-api-openapi.yml
  format: yaml
  label: BombBomb Automations API
  slug: bombbomb-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-automations-api-openapi.yml
- filename: bombbomb-contacts-api-openapi.yml
  format: yaml
  label: BombBomb Contacts API
  slug: bombbomb-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-contacts-api-openapi.yml
- filename: bombbomb-curriculum-api-openapi.yml
  format: yaml
  label: BombBomb Curriculum API
  slug: bombbomb-curriculum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-curriculum-api-openapi.yml
- filename: bombbomb-emails-api-openapi.yml
  format: yaml
  label: BombBomb Emails API
  slug: bombbomb-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-emails-api-openapi.yml
- filename: bombbomb-files-api-openapi.yml
  format: yaml
  label: BombBomb Files API
  slug: bombbomb-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-files-api-openapi.yml
- filename: bombbomb-forms-api-openapi.yml
  format: yaml
  label: BombBomb Forms API
  slug: bombbomb-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-forms-api-openapi.yml
- filename: bombbomb-integrations-api-openapi.yml
  format: yaml
  label: BombBomb Integrations API
  slug: bombbomb-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-integrations-api-openapi.yml
- filename: bombbomb-lists-api-openapi.yml
  format: yaml
  label: BombBomb Lists API
  slug: bombbomb-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-lists-api-openapi.yml
- filename: bombbomb-orders-api-openapi.yml
  format: yaml
  label: BombBomb Orders API
  slug: bombbomb-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-orders-api-openapi.yml
- filename: bombbomb-prompts-api-openapi.yml
  format: yaml
  label: BombBomb Prompts API
  slug: bombbomb-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-prompts-api-openapi.yml
- filename: bombbomb-socials-api-openapi.yml
  format: yaml
  label: BombBomb Socials API
  slug: bombbomb-socials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-socials-api-openapi.yml
- filename: bombbomb-teams-api-openapi.yml
  format: yaml
  label: BombBomb Teams API
  slug: bombbomb-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-teams-api-openapi.yml
- filename: bombbomb-users-api-openapi.yml
  format: yaml
  label: BombBomb Users API
  slug: bombbomb-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-users-api-openapi.yml
- filename: bombbomb-utilities-api-openapi.yml
  format: yaml
  label: BombBomb Utilities API
  slug: bombbomb-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-utilities-api-openapi.yml
- filename: bombbomb-videos-api-openapi.yml
  format: yaml
  label: BombBomb Videos API
  slug: bombbomb-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-videos-api-openapi.yml
- filename: bombbomb-webhooks-api-openapi.yml
  format: yaml
  label: BombBomb Webhooks API
  slug: bombbomb-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BombBomb Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: BombBomb secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: BombBomb
provider_slug: bombbomb
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.bombbomb.com/auth/authorize
    flow: implicit
    scopes: 23
  name: BBOAuth2
  sources:
  - openapi/bombbomb-openapi.yaml
  type: oauth2
slug: bombbomb-authentication
source_filename: bombbomb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/bombbomb-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: BBOAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://app.bombbomb.com/auth/authorize\n    scopes: 23\n  sources:\n  - openapi/bombbomb-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/bombbomb/authentication/bombbomb-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Video Messaging
- Sales
- Marketing
- Human Resources
---
