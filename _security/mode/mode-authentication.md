---
api_key_in: []
api_specs:
- filename: mode-openapi-original.yml
  format: yaml
  label: Mode API
  slug: mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mode/refs/heads/main/openapi/mode-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mode
provider_slug: mode
scheme_count: 1
schemes:
- name: accessTokenAuth
  scheme: basic
  sources:
  - openapi/mode-openapi-original.yml
  type: http
slug: mode-authentication
source_filename: mode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mode-openapi-original.yml\ndocs: https://mode.com/developer/api-reference/authentication/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  notes: >-\n    HTTP Basic authentication. The token (public access key) is used as the username and\n    the secret (private access key, shown only once) as the password; the pair is\n    base64-encoded into an Authorization: Basic <encoded> header. Workspace must be on a\n    paid Mode Business plan to access the API.\ntoken_types:\n- name: Workspace API token\n  scope: workspace\n  notes: >-\n    Created by workspace admins under Workspace Settings > Privacy & Security > API.\n    Grants admin-level workspace access. Cannot be used with cloning reports or invites\n    endpoints.\n- name: Personal API token\n  scope: user\n  notes: >-\n    Legacy option, no longer creatable but still functional; respects the individual\n    user's permissions within the workspace.\n\
  schemes:\n- name: accessTokenAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/mode-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mode/refs/heads/main/authentication/mode-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Business Intelligence
- Analytics
- Data
- Reporting
- Dashboards
- SQL
- Data Stack
---
