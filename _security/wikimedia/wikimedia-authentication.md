---
api_key_in: []
api_specs:
- filename: api.php
  format: yaml
  label: MediaWiki Action API
  slug: mediawiki-action-api
  spec_type: OpenAPI
  url: https://en.wikipedia.org/w/api.php?action=openapi
- filename: wikimedia-rest-api.json
  format: json
  label: Wikimedia REST API (RESTBase)
  slug: wikimedia-rest-api-restbase
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-rest-api.json
- filename: wikimedia-enterprise-api.yaml
  format: yaml
  label: Wikimedia Enterprise API
  slug: wikimedia-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-enterprise-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wikimedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikimedia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wikimedia
provider_slug: wikimedia
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wikimedia-enterprise-api.yaml
  type: http
slug: wikimedia-authentication
source_filename: wikimedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikimedia-enterprise-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wikimedia-enterprise-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/authentication/wikimedia-authentication.yml
summary_line: http · 1 scheme
tags:
- Wikipedia
- Wikimedia
- Encyclopedia
- Open Knowledge
- Content
- Search
- Reference
---
