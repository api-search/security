---
api_key_in: []
api_specs:
- filename: gladly-agents-api-openapi.yml
  format: yaml
  label: Gladly Agents API
  slug: gladly-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-agents-api-openapi.yml
- filename: gladly-answer-management-api-openapi.yml
  format: yaml
  label: Gladly Answer Management API
  slug: gladly-answer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-answer-management-api-openapi.yml
- filename: gladly-audiences-api-openapi.yml
  format: yaml
  label: Gladly Audiences API
  slug: gladly-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-audiences-api-openapi.yml
- filename: gladly-business-hours-api-openapi.yml
  format: yaml
  label: Gladly Business Hours API
  slug: gladly-business-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-business-hours-api-openapi.yml
- filename: gladly-communications-api-openapi.yml
  format: yaml
  label: Gladly Communications API
  slug: gladly-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-communications-api-openapi.yml
- filename: gladly-conversations-api-openapi.yml
  format: yaml
  label: Gladly Conversations API
  slug: gladly-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-conversations-api-openapi.yml
- filename: gladly-customers-api-openapi.yml
  format: yaml
  label: Gladly Customers API
  slug: gladly-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-customers-api-openapi.yml
- filename: gladly-events-api-openapi.yml
  format: yaml
  label: Gladly Events API
  slug: gladly-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-events-api-openapi.yml
- filename: gladly-export-api-openapi.yml
  format: yaml
  label: Gladly Export API
  slug: gladly-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-export-api-openapi.yml
- filename: gladly-freeform-topics-api-openapi.yml
  format: yaml
  label: Gladly Freeform Topics API
  slug: gladly-freeform-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-freeform-topics-api-openapi.yml
- filename: gladly-inboxes-api-openapi.yml
  format: yaml
  label: Gladly Inboxes API
  slug: gladly-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-inboxes-api-openapi.yml
- filename: gladly-organization-api-openapi.yml
  format: yaml
  label: Gladly Organization API
  slug: gladly-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-organization-api-openapi.yml
- filename: gladly-payloads-api-openapi.yml
  format: yaml
  label: Gladly Payloads API
  slug: gladly-payloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-payloads-api-openapi.yml
- filename: gladly-proactive-conversations-api-openapi.yml
  format: yaml
  label: Gladly Proactive Conversations API
  slug: gladly-proactive-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-proactive-conversations-api-openapi.yml
- filename: gladly-public-answer-api-openapi.yml
  format: yaml
  label: Gladly Public Answer API
  slug: gladly-public-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-public-answer-api-openapi.yml
- filename: gladly-reports-api-openapi.yml
  format: yaml
  label: Gladly Reports API
  slug: gladly-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-reports-api-openapi.yml
- filename: gladly-tasks-api-openapi.yml
  format: yaml
  label: Gladly Tasks API
  slug: gladly-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-tasks-api-openapi.yml
- filename: gladly-teams-api-openapi.yml
  format: yaml
  label: Gladly Teams API
  slug: gladly-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-teams-api-openapi.yml
- filename: gladly-topics-api-openapi.yml
  format: yaml
  label: Gladly Topics API
  slug: gladly-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-topics-api-openapi.yml
- filename: gladly-user-identity-api-openapi.yml
  format: yaml
  label: Gladly User Identity API
  slug: gladly-user-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-user-identity-api-openapi.yml
- filename: gladly-webhooks-api-openapi.yml
  format: yaml
  label: Gladly Webhooks API
  slug: gladly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-webhooks-api-openapi.yml
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
