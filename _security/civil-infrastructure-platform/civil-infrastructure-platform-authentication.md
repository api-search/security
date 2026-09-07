---
anonymous_access: false
api_key_in: []
api_specs:
- filename: civil-infrastructure-platform-tec-v1-openapi-original.json
  format: json
  label: CIP Events REST API
  slug: cip-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civil-infrastructure-platform/refs/heads/main/openapi/civil-infrastructure-platform-tec-v1-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Civil Infrastructure Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Civil Infrastructure Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Civil Infrastructure Platform
provider_slug: civil-infrastructure-platform
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/civil-infrastructure-platform-tec-v1-openapi-original.json
  type: http
slug: civil-infrastructure-platform-authentication
source_filename: civil-infrastructure-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/civil-infrastructure-platform-tec-v1-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/civil-infrastructure-platform-tec-v1-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civil-infrastructure-platform/refs/heads/main/authentication/civil-infrastructure-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Embedded
- Industrial
- Infrastructure
- Linux
- Linux Foundation
- Long-Term Support
- Open-Source
---
