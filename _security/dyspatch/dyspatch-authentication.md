---
api_key_in:
- header
api_specs:
- filename: dyspatch-openapi-original.json
  format: json
  label: Dyspatch API
  slug: dyspatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyspatch/refs/heads/main/openapi/dyspatch-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dyspatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dyspatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dyspatch
provider_slug: dyspatch
scheme_count: 1
schemes:
- description: 'Set Bearer followed by your API key as the Authorization header in your

    API requests.


    ```shell

    Authorization: Bearer [example key]

    ```


    Below is an example curl request with an API key in the Authorization header.


    ```shell

    curl --request GET \

    --url https://api.dyspatch.io/templates \

    --header ''Authorization: Bearer [example key]'' \

    --header ''Accept: application/v'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/dyspatch-openapi-original.json
  type: apiKey
slug: dyspatch-authentication
source_filename: dyspatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/dyspatch-openapi-original.json\ndocs: https://docs.dyspatch.io/administration/creating_api_keys/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  detail: >-\n    Single scheme: a static Bearer API key sent in the Authorization header\n    (Authorization: Bearer <key>). API keys are created in the Dyspatch admin\n    dashboard and come in read-only and read & write permission levels. No OAuth\n    2.0, OIDC, or scope surface.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Set Bearer followed by your API key as the Authorization header in your\n    API requests.\n\n    ```shell\n    Authorization: Bearer [example key]\n    ```\n\n    Below is an example curl request with an API key in the Authorization header.\n\n    ```shell\n    curl --request GET \\\n    --url https://api.dyspatch.io/templates \\\n    --header 'Authorization: Bearer [example\
  \ key]' \\\n    --header 'Accept: application/v\n  sources:\n  - openapi/dyspatch-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyspatch/refs/heads/main/authentication/dyspatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Email
- Email Templates
- Marketing
- Messaging
- SMS
- Push Notifications
- Localization
- Content Management
- Developer Tools
---
