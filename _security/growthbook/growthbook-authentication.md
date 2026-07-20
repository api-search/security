---
api_key_in: []
api_specs:
- filename: growthbook-openapi.yaml
  format: yaml
  label: GrowthBook REST API
  slug: growthbook-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthbook/refs/heads/main/openapi/growthbook-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Growthbook Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrowthBook secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GrowthBook
provider_slug: growthbook
scheme_count: 2
schemes:
- description: 'If using Bearer auth, pass the Secret Key as the token:

    ```bash

    curl https://api.growthbook.io/api/v1/features   -H "Authorization: Bearer [example key]"

    ```'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/growthbook-openapi.yaml
  type: http
- description: 'If using HTTP Basic auth, pass the Secret Key as the username and leave the password blank:

    ```bash

    curl https://api.growthbook.io/api/v1/features   -u secret_abc123DEF456:

    # The ":" at the end stops curl from asking for a password

    ```'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/growthbook-openapi.yaml
  type: http
slug: growthbook-authentication
source_filename: growthbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/growthbook-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    If using Bearer auth, pass the Secret Key as the token:\n    ```bash\n    curl https://api.growthbook.io/api/v1/features   -H \"Authorization: Bearer [example key]\"\n    ```\n  sources:\n  - openapi/growthbook-openapi.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    If using HTTP Basic auth, pass the Secret Key as the username and leave the password blank:\n    ```bash\n    curl https://api.growthbook.io/api/v1/features   -u secret_abc123DEF456:\n    # The \":\" at the end stops curl from asking for a password\n    ```\n  sources:\n  - openapi/growthbook-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthbook/refs/heads/main/authentication/growthbook-authentication.yml
summary_line: http · 2 schemes
tags:
- Feature Flags
- Experimentation
- Open Source
- AB Testing
- Analytics
---
