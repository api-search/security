---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Transifex API
  slug: transifex-api
  spec_type: OpenAPI
  url: https://transifex.github.io/openapi/
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
