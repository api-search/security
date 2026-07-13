---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Vespa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vespa secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vespa
provider_slug: vespa
scheme_count: 1
schemes:
- description: Client certificate authentication (Vespa enforces mTLS when configured)
  name: mtls
  sources:
  - openapi/vespa-openapi.yml
  type: mutualTLS
slug: vespa-authentication
source_filename: vespa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vespa-openapi.yml\nsummary:\n  types:\n  - mutualTLS\nschemes:\n- name: mtls\n  type: mutualTLS\n  description: Client certificate authentication (Vespa enforces mTLS when configured)\n  sources:\n  - openapi/vespa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vespa/refs/heads/main/authentication/vespa-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Vector Database
- Search
- Open Source
- Real-Time
- Recommendations
---
