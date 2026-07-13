---
api_key_in: []
api_specs:
- filename: gladly-rest-api-openapi.yml
  format: yaml
  label: Gladly REST API
  slug: gladly-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gladly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gladly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gladly
provider_slug: gladly
scheme_count: 1
schemes:
- description: 'Gladly API uses token-based **Basic Authentication**. API tokens are associated with designated Gladly users.

    To create and use an API token, your user must have the API User permission. An API token can be used to perform any API request without restriction.


    | user name   | password  |

    | ----------- | --------- |

    | agent email | API token |


    The credentials must be passed via an `Authorization` '
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/gladly-rest-api-openapi.yml
  type: http
slug: gladly-authentication
source_filename: gladly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gladly-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: \"Gladly API uses token-based **Basic Authentication**. API tokens are associated\\\n    \\ with designated Gladly users.\\nTo create and use an API token, your user must have the\\\n    \\ API User permission. An API token can be used to perform any API request without restriction.\\n\\\n    \\n| user name   | password  |\\n| ----------- | --------- |\\n| agent email | API token |\\n\\\n    \\nThe credentials must be passed via an `Authorization` \"\n  sources:\n  - openapi/gladly-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/authentication/gladly-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Service
- CX
- Contact Center
- AI Customer Service
- Conversations
- Sidekick AI
- Hero
- Voice
- Chat
- SMS
- Email
- Help Center
- Webhooks
- Knowledge Base
---
