---
api_key_in: []
api_specs:
- filename: cpanel-openapi.yml
  format: yaml
  label: cPanel UAPI
  slug: uapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cpanel Authentication
name_suffix: Authentication
oauth_flows: []
overview: cPanel secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cPanel
provider_slug: cpanel
scheme_count: 2
schemes:
- bearerFormat: cPanel API Token
  description: 'Provide a cPanel API token using

    `Authorization: cpanel <username>:<token>` (cPanel''s documented

    token header format). Standard `Authorization: Bearer` is also

    accepted by some deployments.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cpanel-openapi.yml
  type: http
- description: HTTP Basic Authentication with cPanel account credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cpanel-openapi.yml
  type: http
slug: cpanel-authentication
source_filename: cpanel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cpanel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: cPanel API Token\n  description: |-\n    Provide a cPanel API token using\n    `Authorization: cpanel <username>:<token>` (cPanel's documented\n    token header format). Standard `Authorization: Bearer` is also\n    accepted by some deployments.\n  sources:\n  - openapi/cpanel-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with cPanel account credentials.\n  sources:\n  - openapi/cpanel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/authentication/cpanel-authentication.yml
summary_line: http · 2 schemes
tags:
- Control Panel
- DNS
- Domains
- Email
- Hosting
- Reseller
- Server Administration
- Web Hosting
- WHM
---
