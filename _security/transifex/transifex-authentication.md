---
api_key_in: []
api_specs:
- filename: transifex-activity-reports-api-openapi.yml
  format: yaml
  label: Transifex Activity Reports API
  slug: transifex-activity-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-activity-reports-api-openapi.yml
- filename: transifex-context-screenshots-api-openapi.yml
  format: yaml
  label: Transifex Context Screenshots API
  slug: transifex-context-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-context-screenshots-api-openapi.yml
- filename: transifex-glossaries-api-openapi.yml
  format: yaml
  label: Transifex Glossaries API
  slug: transifex-glossaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-glossaries-api-openapi.yml
- filename: transifex-i18n-formats-api-openapi.yml
  format: yaml
  label: Transifex I18n Formats API
  slug: transifex-i18n-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-i18n-formats-api-openapi.yml
- filename: transifex-languages-api-openapi.yml
  format: yaml
  label: Transifex Languages API
  slug: transifex-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-languages-api-openapi.yml
- filename: transifex-organizations-api-openapi.yml
  format: yaml
  label: Transifex Organizations API
  slug: transifex-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-organizations-api-openapi.yml
- filename: transifex-project-webhooks-api-openapi.yml
  format: yaml
  label: Transifex Project Webhooks API
  slug: transifex-project-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-project-webhooks-api-openapi.yml
- filename: transifex-projects-api-openapi.yml
  format: yaml
  label: Transifex Projects API
  slug: transifex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-projects-api-openapi.yml
- filename: transifex-resource-string-comments-api-openapi.yml
  format: yaml
  label: Transifex Resource String Comments API
  slug: transifex-resource-string-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-resource-string-comments-api-openapi.yml
- filename: transifex-resource-strings-api-openapi.yml
  format: yaml
  label: Transifex Resource Strings API
  slug: transifex-resource-strings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-resource-strings-api-openapi.yml
- filename: transifex-resource-translations-api-openapi.yml
  format: yaml
  label: Transifex Resource Translations API
  slug: transifex-resource-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-resource-translations-api-openapi.yml
- filename: transifex-resources-api-openapi.yml
  format: yaml
  label: Transifex Resources API
  slug: transifex-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-resources-api-openapi.yml
- filename: transifex-statistics-api-openapi.yml
  format: yaml
  label: Transifex Statistics API
  slug: transifex-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-statistics-api-openapi.yml
- filename: transifex-tasks-api-openapi.yml
  format: yaml
  label: Transifex Tasks API
  slug: transifex-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-tasks-api-openapi.yml
- filename: transifex-team-memberships-api-openapi.yml
  format: yaml
  label: Transifex Team Memberships API
  slug: transifex-team-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-team-memberships-api-openapi.yml
- filename: transifex-teams-api-openapi.yml
  format: yaml
  label: Transifex Teams API
  slug: transifex-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-teams-api-openapi.yml
- filename: transifex-translation-memory-api-openapi.yml
  format: yaml
  label: Transifex Translation Memory API
  slug: transifex-translation-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-translation-memory-api-openapi.yml
- filename: transifex-users-api-openapi.yml
  format: yaml
  label: Transifex Users API
  slug: transifex-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/openapi/transifex-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Transifex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transifex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transifex
provider_slug: transifex
scheme_count: 1
schemes:
- description: 'To use the API you need to authenticate your requests using Token Authentication. Specifically, you need to


    * Acquire an authentication token from the Transifex (under user settings)

    * Uses the `Bearer` keyword and  prepend the token when passing the header.


    For example, if the authentication token is `1/0b4e75552e481aeae813aebad53f3de3fcc67ccd`, then the HTTP header should look like this:


    `Aut'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/transifex-transifex-api-openapi.yml
  type: http
slug: transifex-authentication
source_filename: transifex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transifex-transifex-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    To use the API you need to authenticate your requests using Token Authentication. Specifically, you need to\n\n    * Acquire an authentication token from the Transifex (under user settings)\n    * Uses the `Bearer` keyword and  prepend the token when passing the header.\n\n    For example, if the authentication token is `1/0b4e75552e481aeae813aebad53f3de3fcc67ccd`, then the HTTP header should look like this:\n\n    `Aut\n  sources:\n  - openapi/transifex-transifex-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/authentication/transifex-authentication.yml
summary_line: http · 1 scheme
tags:
- Localization
- Translation
- i18n
- l10n
- Language
- Content Management
- Workflow Automation
---
