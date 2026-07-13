---
api_key_in: []
api_specs:
- filename: squid-cache-manager-openapi.yml
  format: yaml
  label: Squid Cache Manager API
  slug: squid-cache-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squid/refs/heads/main/openapi/squid-cache-manager-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Squid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Squid
provider_slug: squid
scheme_count: 1
schemes:
- description: Cache manager password configured via cachemgr_passwd in squid.conf
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/squid-cache-manager-openapi.yml
  type: http
slug: squid-authentication
source_filename: squid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/squid-cache-manager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Cache manager password configured via cachemgr_passwd in squid.conf\n  sources:\n  - openapi/squid-cache-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squid/refs/heads/main/authentication/squid-authentication.yml
summary_line: http · 1 scheme
tags:
- Caching Proxy
- Proxy
- HTTP Proxy
- Web Cache
- Access Control
- Content Filtering
---
