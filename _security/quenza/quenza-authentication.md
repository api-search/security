---
api_key_in: []
api_specs:
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Clients API
  slug: quenza-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Groups API
  slug: quenza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Members API
  slug: quenza-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Tasks API
  slug: quenza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quenza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quenza secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quenza
provider_slug: quenza
scheme_count: 1
schemes:
- description: 'Authenticate using a **Bearer token** in the `Authorization` header:


    ```

    Authorization: Bearer {your-token}

    ```


    You can generate or regenerate your API token in your Quenza workspace under

    **Settings → Developer Tools → API Token**.'
  name: http
  scheme: bearer
  sources:
  - openapi/quenza-openapi.yml
  type: http
slug: quenza-authentication
source_filename: quenza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quenza-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  description: |-\n    Authenticate using a **Bearer token** in the `Authorization` header:\n\n    ```\n    Authorization: Bearer {your-token}\n    ```\n\n    You can generate or regenerate your API token in your Quenza workspace under\n    **Settings → Developer Tools → API Token**.\n  sources:\n  - openapi/quenza-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/authentication/quenza-authentication.yml
summary_line: http · 1 scheme
tags:
- Coaching
- Therapy
- Client Engagement
- Digital Health
- Mental Health
- Practice Management
- Positive Psychology
---
