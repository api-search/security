---
api_key_in: []
api_specs:
- filename: unkey-openapi.yml
  format: yaml
  label: Unkey API
  slug: unkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey/refs/heads/main/openapi/unkey-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unkey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unkey
provider_slug: unkey
scheme_count: 1
schemes:
- bearerFormat: root key
  description: 'Unkey uses API keys (root keys) for authentication. These keys authorize access to management operations in the API.

    To authenticate, include your root key in the Authorization header of each request:

    ```

    Authorization: Bearer unkey_123

    ```

    Root keys have specific permissions attached to them, controlling what operations they can perform. Key permissions follow a hierarchical structure with patter'
  name: rootKey
  scheme: bearer
  sources:
  - openapi/unkey-openapi.yml
  type: http
slug: unkey-authentication
source_filename: unkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unkey-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: rootKey\n  type: http\n  scheme: bearer\n  bearerFormat: root key\n  description: |-\n    Unkey uses API keys (root keys) for authentication. These keys authorize access to management operations in the API.\n    To authenticate, include your root key in the Authorization header of each request:\n    ```\n    Authorization: Bearer unkey_123\n    ```\n    Root keys have specific permissions attached to them, controlling what operations they can perform. Key permissions follow a hierarchical structure with patter\n  sources:\n  - openapi/unkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unkey/refs/heads/main/authentication/unkey-authentication.yml
summary_line: http · 1 scheme
tags:
- API Keys
- Rate Limiting
- Authentication
- Developer Platform
- Access Control
- Identity
- Analytics
---
