---
api_key_in:
- header
api_specs:
- filename: lish-wordpress-openapi.json
  format: json
  label: Lish WordPress REST API
  slug: lish-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-wordpress-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lish secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lish
provider_slug: lish
scheme_count: 1
schemes:
- description: The public read surface documented here requires NO credentials — the live index reports an empty `authentication` object. Authenticated operations use a cookie plus an `X-WP-Nonce` header (same-origin), or HTTP Basic with a WordPress Application Password (`/wp/v2/users/<id>/application-passwords` is present in the live index).
  in: header
  name: anonymous
  parameter: X-WP-Nonce
  sources:
  - openapi/lish-wordpress-openapi.json
  type: apiKey
slug: lish-authentication
source_filename: lish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lish-wordpress-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: anonymous\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: The public read surface documented here requires NO credentials — the live index\n    reports an empty `authentication` object. Authenticated operations use a cookie plus an\n    `X-WP-Nonce` header (same-origin), or HTTP Basic with a WordPress Application Password (`/wp/v2/users/<id>/application-passwords`\n    is present in the live index).\n  sources:\n  - openapi/lish-wordpress-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/authentication/lish-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Catering
- Food and Beverage
- Food Delivery
- Workplace
- Corporate Services
- Content
---
