---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forward-email-account-api-openapi.yml
  format: yaml
  label: Forward Email Account API
  slug: forward-email-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-account-api-openapi.yml
- filename: forward-email-aliases-api-openapi.yml
  format: yaml
  label: Forward Email Aliases API
  slug: forward-email-aliases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-aliases-api-openapi.yml
- filename: forward-email-calendar-events-api-openapi.yml
  format: yaml
  label: Forward Email Calendar Events API
  slug: forward-email-calendar-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-calendar-events-api-openapi.yml
- filename: forward-email-calendars-api-openapi.yml
  format: yaml
  label: Forward Email Calendars API
  slug: forward-email-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-calendars-api-openapi.yml
- filename: forward-email-contacts-api-openapi.yml
  format: yaml
  label: Forward Email Contacts API
  slug: forward-email-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-contacts-api-openapi.yml
- filename: forward-email-domains-api-openapi.yml
  format: yaml
  label: Forward Email Domains API
  slug: forward-email-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-domains-api-openapi.yml
- filename: forward-email-emails-api-openapi.yml
  format: yaml
  label: Forward Email Emails API
  slug: forward-email-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-emails-api-openapi.yml
- filename: forward-email-encrypt-api-openapi.yml
  format: yaml
  label: Forward Email Encrypt API
  slug: forward-email-encrypt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-encrypt-api-openapi.yml
- filename: forward-email-folders-api-openapi.yml
  format: yaml
  label: Forward Email Folders API
  slug: forward-email-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-folders-api-openapi.yml
- filename: forward-email-invites-api-openapi.yml
  format: yaml
  label: Forward Email Invites API
  slug: forward-email-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-invites-api-openapi.yml
- filename: forward-email-logs-api-openapi.yml
  format: yaml
  label: Forward Email Logs API
  slug: forward-email-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-logs-api-openapi.yml
- filename: forward-email-members-api-openapi.yml
  format: yaml
  label: Forward Email Members API
  slug: forward-email-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-members-api-openapi.yml
- filename: forward-email-messages-api-openapi.yml
  format: yaml
  label: Forward Email Messages API
  slug: forward-email-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-messages-api-openapi.yml
- filename: forward-email-push-tokens-api-openapi.yml
  format: yaml
  label: Forward Email Push Tokens API
  slug: forward-email-push-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-push-tokens-api-openapi.yml
- filename: forward-email-sieve-scripts-api-openapi.yml
  format: yaml
  label: Forward Email Sieve Scripts API
  slug: forward-email-sieve-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-sieve-scripts-api-openapi.yml
- filename: forward-email-websockets-api-openapi.yml
  format: yaml
  label: Forward Email WebSockets API
  slug: forward-email-websockets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-websockets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Forward Email Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forward Email secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forward Email
provider_slug: forward-email
scheme_count: 1
schemes:
- description: 'Use your API Key as the **username** for Basic Authentication. Leave the password field empty.


    **Example:**

    If your API Key is `YOUR_API_KEY`, the Base64 encoded value for the `Authorization` header would be `echo -n "YOUR_API_KEY:" | base64`.


    ```http

    Authorization: Basic WU9VUl9BUElfS0VZOg==

    ```'
  name: ApiKeyAuth
  scheme: basic
  sources:
  - openapi/forward-email-openapi.json
  type: http
slug: forward-email-authentication
source_filename: forward-email-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: derived\nsource: openapi/forward-email-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: basic\n  description: |-\n    Use your API Key as the **username** for Basic Authentication. Leave the password field empty.\n\n    **Example:**\n    If your API Key is `YOUR_API_KEY`, the Base64 encoded value for the `Authorization` header would be `echo -n \"YOUR_API_KEY:\" | base64`.\n\n    ```http\n    Authorization: Basic WU9VUl9BUElfS0VZOg==\n    ```\n  sources:\n  - openapi/forward-email-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/forward-email/authentication/forward-email-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Forwarding
- Email Hosting
- Open Source
- API
- Secure Email
---
