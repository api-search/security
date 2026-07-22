---
api_key_in:
- header
api_specs:
- filename: mist-openapi-original.json
  format: json
  label: Juniper Mist Cloud API
  slug: juniper-mist-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mist/refs/heads/main/openapi/mist-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mist secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mist
provider_slug: mist
scheme_count: 2
schemes:
- description: "Preferred authentication method for automation and integrations. Send the API token in the HTTP `Authorization` header.\n\n**Format**:\n  `Authorization: Token {apitoken}`\n\n**Notes**:\n* An API token generated for a specific admin has the same privileges as that admin\n* An API token is automatically removed if it is not used for more than 90 days\n* SSO admins cannot generate admin API tokens. Use orga"
  in: header
  name: apiToken
  parameter: Authorization
  sources:
  - openapi/mist-openapi-original.json
  type: apiKey
- description: 'Session-based authentication for browser or login/password flows. After a successful [Login](/#operations/login) request, Mist returns a `csrftoken` cookie. Send that value in the `X-CSRFToken` header on later API requests that use the login session.


    **Format**:

    ```

    X-CSRFToken: vwvBuq9qkqaKh7lu8tNc0gkvBfEaLAmx

    ```


    For automation, API Token authentication is preferred.'
  in: header
  name: csrfToken
  parameter: X-CSRFToken
  sources:
  - openapi/mist-openapi-original.json
  type: apiKey
slug: mist-authentication
source_filename: mist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mist-openapi-original.json\ndocs: https://www.juniper.net/documentation/us/en/software/mist/automation-integration/topics/task/create-token-for-rest-api.html\nnotes: >-\n  Basic Authentication is deprecated for all Mist API use cases effective\n  September 2026; all integrations must use API tokens. Tokens can be scoped to\n  an admin or an entire org, and are auto-removed after 90 days of non-use.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Preferred authentication method for automation and integrations. Send the API token in the HTTP `Authorization` header.\n\n    **Format**:\n      `Authorization: Token {apitoken}`\n\n    **Notes**:\n    * An API token generated for a specific admin has the same privileges as that admin\n    * An API token is automatically removed if it is not used for more\
  \ than 90 days\n    * SSO admins cannot generate admin API tokens. Use orga\n  sources:\n  - openapi/mist-openapi-original.json\n- name: csrfToken\n  type: apiKey\n  in: header\n  parameter: X-CSRFToken\n  description: |-\n    Session-based authentication for browser or login/password flows. After a successful [Login](/#operations/login) request, Mist returns a `csrftoken` cookie. Send that value in the `X-CSRFToken` header on later API requests that use the login session.\n\n    **Format**:\n    ```\n    X-CSRFToken: vwvBuq9qkqaKh7lu8tNc0gkvBfEaLAmx\n    ```\n\n    For automation, API Token authentication is preferred.\n  sources:\n  - openapi/mist-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mist/refs/heads/main/authentication/mist-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Networking
- Wireless
- Wi-Fi
- Cloud Management
- Artificial Intelligence
- Network Automation
- Location Services
- Webhooks
- Juniper
---
