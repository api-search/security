---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Clojars REST API
  slug: clojars-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clojars Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clojars secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clojars
provider_slug: clojars
scheme_count: 1
schemes:
- description: HTTP Basic authentication using your Clojars username and a deploy token (not your password). Deploy tokens can be created at https://clojars.org/tokens. Required only for write/deploy operations.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
slug: clojars-authentication
source_filename: clojars-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your Clojars username and a deploy token (not\n    your password). Deploy tokens can be created at https://clojars.org/tokens. Required only\n    for write/deploy operations.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/authentication/clojars-authentication.yml
summary_line: http · 1 scheme
tags:
- Clojure
- Package Registry
- Artifact Repository
- Open Source
---
